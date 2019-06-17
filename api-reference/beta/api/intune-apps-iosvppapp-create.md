---
title: Create iosVppApp
description: Создание объекта iosVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 098a671deb94deb501ff3828cd53c7ee8b1bd00b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964936"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="dad02-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="dad02-103">Create iosVppApp</span></span>

> <span data-ttu-id="dad02-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dad02-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dad02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad02-106">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dad02-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dad02-107">Prerequisites</span></span>
<span data-ttu-id="dad02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dad02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad02-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dad02-110">Permission type</span></span>|<span data-ttu-id="dad02-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dad02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dad02-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dad02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dad02-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad02-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dad02-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dad02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dad02-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad02-115">Not supported.</span></span>|
|<span data-ttu-id="dad02-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dad02-116">Application</span></span>|<span data-ttu-id="dad02-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad02-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dad02-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dad02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dad02-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dad02-119">Request headers</span></span>
|<span data-ttu-id="dad02-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dad02-120">Header</span></span>|<span data-ttu-id="dad02-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dad02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dad02-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dad02-122">Authorization</span></span>|<span data-ttu-id="dad02-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dad02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dad02-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dad02-124">Accept</span></span>|<span data-ttu-id="dad02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dad02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dad02-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dad02-126">Request body</span></span>
<span data-ttu-id="dad02-127">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dad02-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="dad02-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="dad02-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="dad02-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dad02-129">Property</span></span>|<span data-ttu-id="dad02-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dad02-130">Type</span></span>|<span data-ttu-id="dad02-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dad02-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dad02-132">id</span><span class="sxs-lookup"><span data-stu-id="dad02-132">id</span></span>|<span data-ttu-id="dad02-133">String</span><span class="sxs-lookup"><span data-stu-id="dad02-133">String</span></span>|<span data-ttu-id="dad02-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dad02-134">Key of the entity.</span></span> <span data-ttu-id="dad02-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dad02-136">displayName</span></span>|<span data-ttu-id="dad02-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dad02-137">String</span></span>|<span data-ttu-id="dad02-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="dad02-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dad02-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-140">description</span><span class="sxs-lookup"><span data-stu-id="dad02-140">description</span></span>|<span data-ttu-id="dad02-141">Строка</span><span class="sxs-lookup"><span data-stu-id="dad02-141">String</span></span>|<span data-ttu-id="dad02-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-142">The description of the app.</span></span> <span data-ttu-id="dad02-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-144">publisher</span><span class="sxs-lookup"><span data-stu-id="dad02-144">publisher</span></span>|<span data-ttu-id="dad02-145">String</span><span class="sxs-lookup"><span data-stu-id="dad02-145">String</span></span>|<span data-ttu-id="dad02-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-146">The publisher of the app.</span></span> <span data-ttu-id="dad02-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dad02-148">largeIcon</span></span>|[<span data-ttu-id="dad02-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dad02-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dad02-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="dad02-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dad02-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dad02-152">createdDateTime</span></span>|<span data-ttu-id="dad02-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dad02-153">DateTimeOffset</span></span>|<span data-ttu-id="dad02-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-154">The date and time the app was created.</span></span> <span data-ttu-id="dad02-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dad02-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dad02-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dad02-157">DateTimeOffset</span></span>|<span data-ttu-id="dad02-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dad02-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dad02-160">isFeatured</span></span>|<span data-ttu-id="dad02-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dad02-161">Boolean</span></span>|<span data-ttu-id="dad02-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dad02-163">privacyInformationUrl</span></span>|<span data-ttu-id="dad02-164">String</span><span class="sxs-lookup"><span data-stu-id="dad02-164">String</span></span>|<span data-ttu-id="dad02-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="dad02-165">The privacy statement Url.</span></span> <span data-ttu-id="dad02-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dad02-167">informationUrl</span></span>|<span data-ttu-id="dad02-168">String</span><span class="sxs-lookup"><span data-stu-id="dad02-168">String</span></span>|<span data-ttu-id="dad02-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="dad02-169">The more information Url.</span></span> <span data-ttu-id="dad02-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-171">owner</span><span class="sxs-lookup"><span data-stu-id="dad02-171">owner</span></span>|<span data-ttu-id="dad02-172">String</span><span class="sxs-lookup"><span data-stu-id="dad02-172">String</span></span>|<span data-ttu-id="dad02-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-173">The owner of the app.</span></span> <span data-ttu-id="dad02-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-175">developer</span><span class="sxs-lookup"><span data-stu-id="dad02-175">developer</span></span>|<span data-ttu-id="dad02-176">String</span><span class="sxs-lookup"><span data-stu-id="dad02-176">String</span></span>|<span data-ttu-id="dad02-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-177">The developer of the app.</span></span> <span data-ttu-id="dad02-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-179">notes</span><span class="sxs-lookup"><span data-stu-id="dad02-179">notes</span></span>|<span data-ttu-id="dad02-180">String</span><span class="sxs-lookup"><span data-stu-id="dad02-180">String</span></span>|<span data-ttu-id="dad02-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-181">Notes for the app.</span></span> <span data-ttu-id="dad02-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="dad02-183">uploadState</span></span>|<span data-ttu-id="dad02-184">Int32</span><span class="sxs-lookup"><span data-stu-id="dad02-184">Int32</span></span>|<span data-ttu-id="dad02-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="dad02-185">The upload state.</span></span> <span data-ttu-id="dad02-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="dad02-187">publishingState</span></span>|[<span data-ttu-id="dad02-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="dad02-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dad02-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-189">The publishing state for the app.</span></span> <span data-ttu-id="dad02-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="dad02-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dad02-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dad02-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dad02-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dad02-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dad02-193">isAssigned</span></span>|<span data-ttu-id="dad02-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dad02-194">Boolean</span></span>|<span data-ttu-id="dad02-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="dad02-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="dad02-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dad02-197">roleScopeTagIds</span></span>|<span data-ttu-id="dad02-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dad02-198">String collection</span></span>|<span data-ttu-id="dad02-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="dad02-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="dad02-201">dependentAppCount</span></span>|<span data-ttu-id="dad02-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dad02-202">Int32</span></span>|<span data-ttu-id="dad02-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="dad02-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="dad02-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dad02-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dad02-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dad02-205">usedLicenseCount</span></span>|<span data-ttu-id="dad02-206">Int32</span><span class="sxs-lookup"><span data-stu-id="dad02-206">Int32</span></span>|<span data-ttu-id="dad02-207">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="dad02-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="dad02-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dad02-208">totalLicenseCount</span></span>|<span data-ttu-id="dad02-209">Int32</span><span class="sxs-lookup"><span data-stu-id="dad02-209">Int32</span></span>|<span data-ttu-id="dad02-210">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="dad02-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="dad02-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="dad02-211">releaseDateTime</span></span>|<span data-ttu-id="dad02-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dad02-212">DateTimeOffset</span></span>|<span data-ttu-id="dad02-213">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="dad02-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="dad02-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dad02-214">appStoreUrl</span></span>|<span data-ttu-id="dad02-215">String</span><span class="sxs-lookup"><span data-stu-id="dad02-215">String</span></span>|<span data-ttu-id="dad02-216">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="dad02-216">The store URL.</span></span>|
|<span data-ttu-id="dad02-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="dad02-217">licensingType</span></span>|[<span data-ttu-id="dad02-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="dad02-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="dad02-219">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="dad02-219">The supported License Type.</span></span>|
|<span data-ttu-id="dad02-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="dad02-220">applicableDeviceType</span></span>|[<span data-ttu-id="dad02-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="dad02-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="dad02-222">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="dad02-222">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="dad02-223">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="dad02-223">vppTokenOrganizationName</span></span>|<span data-ttu-id="dad02-224">String</span><span class="sxs-lookup"><span data-stu-id="dad02-224">String</span></span>|<span data-ttu-id="dad02-225">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="dad02-225">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="dad02-226">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="dad02-226">vppTokenAccountType</span></span>|[<span data-ttu-id="dad02-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="dad02-227">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="dad02-228">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="dad02-228">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="dad02-229">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="dad02-229">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="dad02-230">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="dad02-230">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="dad02-231">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="dad02-231">vppTokenAppleId</span></span>|<span data-ttu-id="dad02-232">String</span><span class="sxs-lookup"><span data-stu-id="dad02-232">String</span></span>|<span data-ttu-id="dad02-233">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="dad02-233">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="dad02-234">bundleId</span><span class="sxs-lookup"><span data-stu-id="dad02-234">bundleId</span></span>|<span data-ttu-id="dad02-235">String</span><span class="sxs-lookup"><span data-stu-id="dad02-235">String</span></span>|<span data-ttu-id="dad02-236">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dad02-236">The Identity Name.</span></span>|
|<span data-ttu-id="dad02-237">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="dad02-237">vppTokenId</span></span>|<span data-ttu-id="dad02-238">String</span><span class="sxs-lookup"><span data-stu-id="dad02-238">String</span></span>|<span data-ttu-id="dad02-239">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="dad02-239">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="dad02-240">Ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="dad02-240">revokeLicenseActionResults</span></span>|<span data-ttu-id="dad02-241">Коллекция [иосвппаппревокелиценсесактионресулт](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dad02-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="dad02-242">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="dad02-242">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="dad02-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="dad02-243">Response</span></span>
<span data-ttu-id="dad02-244">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dad02-244">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dad02-245">Пример</span><span class="sxs-lookup"><span data-stu-id="dad02-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="dad02-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="dad02-246">Request</span></span>
<span data-ttu-id="dad02-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dad02-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1999

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="dad02-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="dad02-248">Response</span></span>
<span data-ttu-id="dad02-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dad02-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2171

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
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





