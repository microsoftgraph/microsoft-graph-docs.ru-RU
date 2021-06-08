---
title: Create iosVppApp
description: Создание объекта iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6c856f3dc32b3166909ededa954ba7fa0636b56
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757327"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="d67a8-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="d67a8-103">Create iosVppApp</span></span>

<span data-ttu-id="d67a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d67a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d67a8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d67a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d67a8-106">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d67a8-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d67a8-107">Prerequisites</span></span>
<span data-ttu-id="d67a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d67a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d67a8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d67a8-110">Permission type</span></span>|<span data-ttu-id="d67a8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d67a8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d67a8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d67a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d67a8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d67a8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d67a8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d67a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d67a8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d67a8-115">Not supported.</span></span>|
|<span data-ttu-id="d67a8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d67a8-116">Application</span></span>|<span data-ttu-id="d67a8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d67a8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d67a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d67a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d67a8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d67a8-119">Request headers</span></span>
|<span data-ttu-id="d67a8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d67a8-120">Header</span></span>|<span data-ttu-id="d67a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d67a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d67a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d67a8-122">Authorization</span></span>|<span data-ttu-id="d67a8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d67a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d67a8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d67a8-124">Accept</span></span>|<span data-ttu-id="d67a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d67a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d67a8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d67a8-126">Request body</span></span>
<span data-ttu-id="d67a8-127">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d67a8-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="d67a8-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="d67a8-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="d67a8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d67a8-129">Property</span></span>|<span data-ttu-id="d67a8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d67a8-130">Type</span></span>|<span data-ttu-id="d67a8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d67a8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d67a8-132">id</span><span class="sxs-lookup"><span data-stu-id="d67a8-132">id</span></span>|<span data-ttu-id="d67a8-133">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-133">String</span></span>|<span data-ttu-id="d67a8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d67a8-134">Key of the entity.</span></span> <span data-ttu-id="d67a8-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d67a8-136">displayName</span></span>|<span data-ttu-id="d67a8-137">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-137">String</span></span>|<span data-ttu-id="d67a8-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d67a8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d67a8-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-140">description</span><span class="sxs-lookup"><span data-stu-id="d67a8-140">description</span></span>|<span data-ttu-id="d67a8-141">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-141">String</span></span>|<span data-ttu-id="d67a8-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-142">The description of the app.</span></span> <span data-ttu-id="d67a8-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d67a8-144">publisher</span></span>|<span data-ttu-id="d67a8-145">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-145">String</span></span>|<span data-ttu-id="d67a8-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-146">The publisher of the app.</span></span> <span data-ttu-id="d67a8-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d67a8-148">largeIcon</span></span>|[<span data-ttu-id="d67a8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d67a8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d67a8-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d67a8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d67a8-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d67a8-152">createdDateTime</span></span>|<span data-ttu-id="d67a8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d67a8-153">DateTimeOffset</span></span>|<span data-ttu-id="d67a8-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-154">The date and time the app was created.</span></span> <span data-ttu-id="d67a8-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d67a8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d67a8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d67a8-157">DateTimeOffset</span></span>|<span data-ttu-id="d67a8-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d67a8-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d67a8-160">isFeatured</span></span>|<span data-ttu-id="d67a8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d67a8-161">Boolean</span></span>|<span data-ttu-id="d67a8-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d67a8-163">privacyInformationUrl</span></span>|<span data-ttu-id="d67a8-164">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-164">String</span></span>|<span data-ttu-id="d67a8-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d67a8-165">The privacy statement Url.</span></span> <span data-ttu-id="d67a8-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d67a8-167">informationUrl</span></span>|<span data-ttu-id="d67a8-168">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-168">String</span></span>|<span data-ttu-id="d67a8-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d67a8-169">The more information Url.</span></span> <span data-ttu-id="d67a8-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-171">owner</span><span class="sxs-lookup"><span data-stu-id="d67a8-171">owner</span></span>|<span data-ttu-id="d67a8-172">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-172">String</span></span>|<span data-ttu-id="d67a8-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-173">The owner of the app.</span></span> <span data-ttu-id="d67a8-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-175">developer</span><span class="sxs-lookup"><span data-stu-id="d67a8-175">developer</span></span>|<span data-ttu-id="d67a8-176">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-176">String</span></span>|<span data-ttu-id="d67a8-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-177">The developer of the app.</span></span> <span data-ttu-id="d67a8-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-179">notes</span><span class="sxs-lookup"><span data-stu-id="d67a8-179">notes</span></span>|<span data-ttu-id="d67a8-180">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-180">String</span></span>|<span data-ttu-id="d67a8-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-181">Notes for the app.</span></span> <span data-ttu-id="d67a8-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d67a8-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="d67a8-183">publishingState</span></span>|[<span data-ttu-id="d67a8-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d67a8-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d67a8-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-185">The publishing state for the app.</span></span> <span data-ttu-id="d67a8-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d67a8-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d67a8-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d67a8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d67a8-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d67a8-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d67a8-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d67a8-189">usedLicenseCount</span></span>|<span data-ttu-id="d67a8-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d67a8-190">Int32</span></span>|<span data-ttu-id="d67a8-191">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d67a8-191">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="d67a8-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d67a8-192">totalLicenseCount</span></span>|<span data-ttu-id="d67a8-193">Int32</span><span class="sxs-lookup"><span data-stu-id="d67a8-193">Int32</span></span>|<span data-ttu-id="d67a8-194">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d67a8-194">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="d67a8-195">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="d67a8-195">releaseDateTime</span></span>|<span data-ttu-id="d67a8-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d67a8-196">DateTimeOffset</span></span>|<span data-ttu-id="d67a8-197">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="d67a8-197">The VPP application release date and time.</span></span>|
|<span data-ttu-id="d67a8-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d67a8-198">appStoreUrl</span></span>|<span data-ttu-id="d67a8-199">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-199">String</span></span>|<span data-ttu-id="d67a8-200">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="d67a8-200">The store URL.</span></span>|
|<span data-ttu-id="d67a8-201">licensingType</span><span class="sxs-lookup"><span data-stu-id="d67a8-201">licensingType</span></span>|[<span data-ttu-id="d67a8-202">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="d67a8-202">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="d67a8-203">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="d67a8-203">The supported License Type.</span></span>|
|<span data-ttu-id="d67a8-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d67a8-204">applicableDeviceType</span></span>|[<span data-ttu-id="d67a8-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d67a8-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d67a8-206">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="d67a8-206">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="d67a8-207">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="d67a8-207">vppTokenOrganizationName</span></span>|<span data-ttu-id="d67a8-208">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-208">String</span></span>|<span data-ttu-id="d67a8-209">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d67a8-209">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="d67a8-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="d67a8-210">vppTokenAccountType</span></span>|[<span data-ttu-id="d67a8-211">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="d67a8-211">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="d67a8-212">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d67a8-212">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="d67a8-213">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="d67a8-213">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="d67a8-214">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="d67a8-214">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="d67a8-215">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="d67a8-215">vppTokenAppleId</span></span>|<span data-ttu-id="d67a8-216">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-216">String</span></span>|<span data-ttu-id="d67a8-217">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d67a8-217">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="d67a8-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="d67a8-218">bundleId</span></span>|<span data-ttu-id="d67a8-219">String</span><span class="sxs-lookup"><span data-stu-id="d67a8-219">String</span></span>|<span data-ttu-id="d67a8-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d67a8-220">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="d67a8-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="d67a8-221">Response</span></span>
<span data-ttu-id="d67a8-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d67a8-222">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d67a8-223">Пример</span><span class="sxs-lookup"><span data-stu-id="d67a8-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="d67a8-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="d67a8-224">Request</span></span>
<span data-ttu-id="d67a8-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d67a8-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d67a8-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="d67a8-226">Response</span></span>
<span data-ttu-id="d67a8-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d67a8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




