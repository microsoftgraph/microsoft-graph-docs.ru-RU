---
title: Create iosVppApp
description: Создание объекта iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a883b237017e4654bd2458bd81a2e78f357d38b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441006"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="5c8e6-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="5c8e6-103">Create iosVppApp</span></span>

<span data-ttu-id="5c8e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c8e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c8e6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c8e6-106">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c8e6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8e6-107">Prerequisites</span></span>
<span data-ttu-id="5c8e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c8e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c8e6-110">Permission type</span></span>|<span data-ttu-id="5c8e6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c8e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c8e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c8e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c8e6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c8e6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c8e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c8e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c8e6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-115">Not supported.</span></span>|
|<span data-ttu-id="5c8e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c8e6-116">Application</span></span>|<span data-ttu-id="5c8e6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c8e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c8e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5c8e6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5c8e6-119">Request headers</span></span>
|<span data-ttu-id="5c8e6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c8e6-120">Header</span></span>|<span data-ttu-id="5c8e6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c8e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c8e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c8e6-122">Authorization</span></span>|<span data-ttu-id="5c8e6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c8e6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c8e6-124">Accept</span></span>|<span data-ttu-id="5c8e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c8e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c8e6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c8e6-126">Request body</span></span>
<span data-ttu-id="5c8e6-127">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="5c8e6-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="5c8e6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c8e6-129">Property</span></span>|<span data-ttu-id="5c8e6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c8e6-130">Type</span></span>|<span data-ttu-id="5c8e6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c8e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c8e6-132">id</span><span class="sxs-lookup"><span data-stu-id="5c8e6-132">id</span></span>|<span data-ttu-id="5c8e6-133">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-133">String</span></span>|<span data-ttu-id="5c8e6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-134">Key of the entity.</span></span> <span data-ttu-id="5c8e6-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5c8e6-136">displayName</span></span>|<span data-ttu-id="5c8e6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5c8e6-137">String</span></span>|<span data-ttu-id="5c8e6-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c8e6-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-140">description</span><span class="sxs-lookup"><span data-stu-id="5c8e6-140">description</span></span>|<span data-ttu-id="5c8e6-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5c8e6-141">String</span></span>|<span data-ttu-id="5c8e6-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-142">The description of the app.</span></span> <span data-ttu-id="5c8e6-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="5c8e6-144">publisher</span></span>|<span data-ttu-id="5c8e6-145">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-145">String</span></span>|<span data-ttu-id="5c8e6-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-146">The publisher of the app.</span></span> <span data-ttu-id="5c8e6-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c8e6-148">largeIcon</span></span>|[<span data-ttu-id="5c8e6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c8e6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c8e6-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c8e6-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c8e6-152">createdDateTime</span></span>|<span data-ttu-id="5c8e6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c8e6-153">DateTimeOffset</span></span>|<span data-ttu-id="5c8e6-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-154">The date and time the app was created.</span></span> <span data-ttu-id="5c8e6-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c8e6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5c8e6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c8e6-157">DateTimeOffset</span></span>|<span data-ttu-id="5c8e6-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5c8e6-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c8e6-160">isFeatured</span></span>|<span data-ttu-id="5c8e6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c8e6-161">Boolean</span></span>|<span data-ttu-id="5c8e6-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c8e6-163">privacyInformationUrl</span></span>|<span data-ttu-id="5c8e6-164">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-164">String</span></span>|<span data-ttu-id="5c8e6-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-165">The privacy statement Url.</span></span> <span data-ttu-id="5c8e6-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c8e6-167">informationUrl</span></span>|<span data-ttu-id="5c8e6-168">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-168">String</span></span>|<span data-ttu-id="5c8e6-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-169">The more information Url.</span></span> <span data-ttu-id="5c8e6-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-171">owner</span><span class="sxs-lookup"><span data-stu-id="5c8e6-171">owner</span></span>|<span data-ttu-id="5c8e6-172">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-172">String</span></span>|<span data-ttu-id="5c8e6-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-173">The owner of the app.</span></span> <span data-ttu-id="5c8e6-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-175">developer</span><span class="sxs-lookup"><span data-stu-id="5c8e6-175">developer</span></span>|<span data-ttu-id="5c8e6-176">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-176">String</span></span>|<span data-ttu-id="5c8e6-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-177">The developer of the app.</span></span> <span data-ttu-id="5c8e6-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-179">notes</span><span class="sxs-lookup"><span data-stu-id="5c8e6-179">notes</span></span>|<span data-ttu-id="5c8e6-180">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-180">String</span></span>|<span data-ttu-id="5c8e6-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-181">Notes for the app.</span></span> <span data-ttu-id="5c8e6-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c8e6-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c8e6-183">publishingState</span></span>|[<span data-ttu-id="5c8e6-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="5c8e6-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c8e6-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-185">The publishing state for the app.</span></span> <span data-ttu-id="5c8e6-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c8e6-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c8e6-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5c8e6-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c8e6-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5c8e6-189">usedLicenseCount</span></span>|<span data-ttu-id="5c8e6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="5c8e6-190">Int32</span></span>|<span data-ttu-id="5c8e6-191">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-191">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="5c8e6-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5c8e6-192">totalLicenseCount</span></span>|<span data-ttu-id="5c8e6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="5c8e6-193">Int32</span></span>|<span data-ttu-id="5c8e6-194">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-194">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="5c8e6-195">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="5c8e6-195">releaseDateTime</span></span>|<span data-ttu-id="5c8e6-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c8e6-196">DateTimeOffset</span></span>|<span data-ttu-id="5c8e6-197">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-197">The VPP application release date and time.</span></span>|
|<span data-ttu-id="5c8e6-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5c8e6-198">appStoreUrl</span></span>|<span data-ttu-id="5c8e6-199">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-199">String</span></span>|<span data-ttu-id="5c8e6-200">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-200">The store URL.</span></span>|
|<span data-ttu-id="5c8e6-201">licensingType</span><span class="sxs-lookup"><span data-stu-id="5c8e6-201">licensingType</span></span>|[<span data-ttu-id="5c8e6-202">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="5c8e6-202">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="5c8e6-203">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-203">The supported License Type.</span></span>|
|<span data-ttu-id="5c8e6-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5c8e6-204">applicableDeviceType</span></span>|[<span data-ttu-id="5c8e6-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5c8e6-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5c8e6-206">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-206">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="5c8e6-207">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="5c8e6-207">vppTokenOrganizationName</span></span>|<span data-ttu-id="5c8e6-208">Строка</span><span class="sxs-lookup"><span data-stu-id="5c8e6-208">String</span></span>|<span data-ttu-id="5c8e6-209">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-209">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="5c8e6-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="5c8e6-210">vppTokenAccountType</span></span>|[<span data-ttu-id="5c8e6-211">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="5c8e6-211">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="5c8e6-212">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-212">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="5c8e6-213">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-213">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="5c8e6-214">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-214">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="5c8e6-215">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="5c8e6-215">vppTokenAppleId</span></span>|<span data-ttu-id="5c8e6-216">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-216">String</span></span>|<span data-ttu-id="5c8e6-217">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-217">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5c8e6-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="5c8e6-218">bundleId</span></span>|<span data-ttu-id="5c8e6-219">String</span><span class="sxs-lookup"><span data-stu-id="5c8e6-219">String</span></span>|<span data-ttu-id="5c8e6-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-220">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="5c8e6-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c8e6-221">Response</span></span>
<span data-ttu-id="5c8e6-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-222">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c8e6-223">Пример</span><span class="sxs-lookup"><span data-stu-id="5c8e6-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c8e6-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c8e6-224">Request</span></span>
<span data-ttu-id="5c8e6-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="5c8e6-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c8e6-226">Response</span></span>
<span data-ttu-id="5c8e6-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c8e6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






