---
title: Update iosVppApp
description: Обновление свойств объекта iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e7b6302aae55b63a2e2faf327f2f82a030894bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456128"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="dff4f-103">Update iosVppApp</span><span class="sxs-lookup"><span data-stu-id="dff4f-103">Update iosVppApp</span></span>

<span data-ttu-id="dff4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dff4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dff4f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dff4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dff4f-106">Обновление свойств объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-106">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dff4f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dff4f-107">Prerequisites</span></span>
<span data-ttu-id="dff4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dff4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dff4f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dff4f-110">Permission type</span></span>|<span data-ttu-id="dff4f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dff4f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dff4f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dff4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dff4f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dff4f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dff4f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dff4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dff4f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dff4f-115">Not supported.</span></span>|
|<span data-ttu-id="dff4f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dff4f-116">Application</span></span>|<span data-ttu-id="dff4f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dff4f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dff4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dff4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="dff4f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dff4f-119">Request headers</span></span>
|<span data-ttu-id="dff4f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dff4f-120">Header</span></span>|<span data-ttu-id="dff4f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dff4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dff4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dff4f-122">Authorization</span></span>|<span data-ttu-id="dff4f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dff4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dff4f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dff4f-124">Accept</span></span>|<span data-ttu-id="dff4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dff4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dff4f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dff4f-126">Request body</span></span>
<span data-ttu-id="dff4f-127">В теле запроса добавьте представление объекта [iosVppApp](../resources/intune-apps-iosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dff4f-127">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="dff4f-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-128">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="dff4f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dff4f-129">Property</span></span>|<span data-ttu-id="dff4f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dff4f-130">Type</span></span>|<span data-ttu-id="dff4f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dff4f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff4f-132">id</span><span class="sxs-lookup"><span data-stu-id="dff4f-132">id</span></span>|<span data-ttu-id="dff4f-133">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-133">String</span></span>|<span data-ttu-id="dff4f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dff4f-134">Key of the entity.</span></span> <span data-ttu-id="dff4f-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dff4f-136">displayName</span></span>|<span data-ttu-id="dff4f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dff4f-137">String</span></span>|<span data-ttu-id="dff4f-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="dff4f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dff4f-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-140">description</span><span class="sxs-lookup"><span data-stu-id="dff4f-140">description</span></span>|<span data-ttu-id="dff4f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="dff4f-141">String</span></span>|<span data-ttu-id="dff4f-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-142">The description of the app.</span></span> <span data-ttu-id="dff4f-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="dff4f-144">publisher</span></span>|<span data-ttu-id="dff4f-145">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-145">String</span></span>|<span data-ttu-id="dff4f-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-146">The publisher of the app.</span></span> <span data-ttu-id="dff4f-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dff4f-148">largeIcon</span></span>|[<span data-ttu-id="dff4f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dff4f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dff4f-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="dff4f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dff4f-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dff4f-152">createdDateTime</span></span>|<span data-ttu-id="dff4f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dff4f-153">DateTimeOffset</span></span>|<span data-ttu-id="dff4f-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-154">The date and time the app was created.</span></span> <span data-ttu-id="dff4f-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dff4f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dff4f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dff4f-157">DateTimeOffset</span></span>|<span data-ttu-id="dff4f-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dff4f-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dff4f-160">isFeatured</span></span>|<span data-ttu-id="dff4f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dff4f-161">Boolean</span></span>|<span data-ttu-id="dff4f-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dff4f-163">privacyInformationUrl</span></span>|<span data-ttu-id="dff4f-164">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-164">String</span></span>|<span data-ttu-id="dff4f-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="dff4f-165">The privacy statement Url.</span></span> <span data-ttu-id="dff4f-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dff4f-167">informationUrl</span></span>|<span data-ttu-id="dff4f-168">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-168">String</span></span>|<span data-ttu-id="dff4f-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="dff4f-169">The more information Url.</span></span> <span data-ttu-id="dff4f-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-171">owner</span><span class="sxs-lookup"><span data-stu-id="dff4f-171">owner</span></span>|<span data-ttu-id="dff4f-172">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-172">String</span></span>|<span data-ttu-id="dff4f-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-173">The owner of the app.</span></span> <span data-ttu-id="dff4f-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-175">developer</span><span class="sxs-lookup"><span data-stu-id="dff4f-175">developer</span></span>|<span data-ttu-id="dff4f-176">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-176">String</span></span>|<span data-ttu-id="dff4f-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-177">The developer of the app.</span></span> <span data-ttu-id="dff4f-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-179">notes</span><span class="sxs-lookup"><span data-stu-id="dff4f-179">notes</span></span>|<span data-ttu-id="dff4f-180">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-180">String</span></span>|<span data-ttu-id="dff4f-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-181">Notes for the app.</span></span> <span data-ttu-id="dff4f-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dff4f-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="dff4f-183">publishingState</span></span>|[<span data-ttu-id="dff4f-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="dff4f-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dff4f-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-185">The publishing state for the app.</span></span> <span data-ttu-id="dff4f-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="dff4f-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dff4f-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dff4f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dff4f-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dff4f-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dff4f-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dff4f-189">usedLicenseCount</span></span>|<span data-ttu-id="dff4f-190">Int32</span><span class="sxs-lookup"><span data-stu-id="dff4f-190">Int32</span></span>|<span data-ttu-id="dff4f-191">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="dff4f-191">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="dff4f-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dff4f-192">totalLicenseCount</span></span>|<span data-ttu-id="dff4f-193">Int32</span><span class="sxs-lookup"><span data-stu-id="dff4f-193">Int32</span></span>|<span data-ttu-id="dff4f-194">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="dff4f-194">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="dff4f-195">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="dff4f-195">releaseDateTime</span></span>|<span data-ttu-id="dff4f-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dff4f-196">DateTimeOffset</span></span>|<span data-ttu-id="dff4f-197">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="dff4f-197">The VPP application release date and time.</span></span>|
|<span data-ttu-id="dff4f-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dff4f-198">appStoreUrl</span></span>|<span data-ttu-id="dff4f-199">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-199">String</span></span>|<span data-ttu-id="dff4f-200">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="dff4f-200">The store URL.</span></span>|
|<span data-ttu-id="dff4f-201">licensingType</span><span class="sxs-lookup"><span data-stu-id="dff4f-201">licensingType</span></span>|[<span data-ttu-id="dff4f-202">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="dff4f-202">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="dff4f-203">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="dff4f-203">The supported License Type.</span></span>|
|<span data-ttu-id="dff4f-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="dff4f-204">applicableDeviceType</span></span>|[<span data-ttu-id="dff4f-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="dff4f-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="dff4f-206">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="dff4f-206">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="dff4f-207">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="dff4f-207">vppTokenOrganizationName</span></span>|<span data-ttu-id="dff4f-208">Строка</span><span class="sxs-lookup"><span data-stu-id="dff4f-208">String</span></span>|<span data-ttu-id="dff4f-209">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="dff4f-209">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="dff4f-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="dff4f-210">vppTokenAccountType</span></span>|[<span data-ttu-id="dff4f-211">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="dff4f-211">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="dff4f-212">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="dff4f-212">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="dff4f-213">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="dff4f-213">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="dff4f-214">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="dff4f-214">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="dff4f-215">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="dff4f-215">vppTokenAppleId</span></span>|<span data-ttu-id="dff4f-216">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-216">String</span></span>|<span data-ttu-id="dff4f-217">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="dff4f-217">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="dff4f-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="dff4f-218">bundleId</span></span>|<span data-ttu-id="dff4f-219">String</span><span class="sxs-lookup"><span data-stu-id="dff4f-219">String</span></span>|<span data-ttu-id="dff4f-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dff4f-220">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="dff4f-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="dff4f-221">Response</span></span>
<span data-ttu-id="dff4f-222">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dff4f-222">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dff4f-223">Пример</span><span class="sxs-lookup"><span data-stu-id="dff4f-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="dff4f-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="dff4f-224">Request</span></span>
<span data-ttu-id="dff4f-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dff4f-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dff4f-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="dff4f-226">Response</span></span>
<span data-ttu-id="dff4f-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dff4f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






