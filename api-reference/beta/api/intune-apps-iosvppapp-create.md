---
title: Create iosVppApp
description: Создание объекта iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b41bc2c51b82a46a4f10c0396f104fe73a08f0f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141848"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="f61d2-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="f61d2-103">Create iosVppApp</span></span>

> <span data-ttu-id="f61d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f61d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f61d2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f61d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f61d2-106">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f61d2-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f61d2-107">Prerequisites</span></span>
<span data-ttu-id="f61d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f61d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f61d2-110">Permission type</span></span>|<span data-ttu-id="f61d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f61d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f61d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f61d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f61d2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f61d2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f61d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f61d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f61d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f61d2-115">Not supported.</span></span>|
|<span data-ttu-id="f61d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f61d2-116">Application</span></span>|<span data-ttu-id="f61d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f61d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f61d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f61d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f61d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f61d2-119">Request headers</span></span>
|<span data-ttu-id="f61d2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f61d2-120">Header</span></span>|<span data-ttu-id="f61d2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f61d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f61d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f61d2-122">Authorization</span></span>|<span data-ttu-id="f61d2-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f61d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f61d2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f61d2-124">Accept</span></span>|<span data-ttu-id="f61d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f61d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f61d2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f61d2-126">Request body</span></span>
<span data-ttu-id="f61d2-127">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f61d2-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="f61d2-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="f61d2-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="f61d2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f61d2-129">Property</span></span>|<span data-ttu-id="f61d2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f61d2-130">Type</span></span>|<span data-ttu-id="f61d2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f61d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f61d2-132">id</span><span class="sxs-lookup"><span data-stu-id="f61d2-132">id</span></span>|<span data-ttu-id="f61d2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f61d2-133">String</span></span>|<span data-ttu-id="f61d2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f61d2-134">Key of the entity.</span></span> <span data-ttu-id="f61d2-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f61d2-136">displayName</span></span>|<span data-ttu-id="f61d2-137">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-137">String</span></span>|<span data-ttu-id="f61d2-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f61d2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f61d2-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-140">description</span><span class="sxs-lookup"><span data-stu-id="f61d2-140">description</span></span>|<span data-ttu-id="f61d2-141">Строка</span><span class="sxs-lookup"><span data-stu-id="f61d2-141">String</span></span>|<span data-ttu-id="f61d2-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-142">The description of the app.</span></span> <span data-ttu-id="f61d2-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f61d2-144">publisher</span></span>|<span data-ttu-id="f61d2-145">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-145">String</span></span>|<span data-ttu-id="f61d2-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-146">The publisher of the app.</span></span> <span data-ttu-id="f61d2-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f61d2-148">largeIcon</span></span>|[<span data-ttu-id="f61d2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f61d2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f61d2-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f61d2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f61d2-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f61d2-152">createdDateTime</span></span>|<span data-ttu-id="f61d2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f61d2-153">DateTimeOffset</span></span>|<span data-ttu-id="f61d2-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-154">The date and time the app was created.</span></span> <span data-ttu-id="f61d2-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f61d2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f61d2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f61d2-157">DateTimeOffset</span></span>|<span data-ttu-id="f61d2-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f61d2-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f61d2-160">isFeatured</span></span>|<span data-ttu-id="f61d2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f61d2-161">Boolean</span></span>|<span data-ttu-id="f61d2-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f61d2-163">privacyInformationUrl</span></span>|<span data-ttu-id="f61d2-164">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-164">String</span></span>|<span data-ttu-id="f61d2-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f61d2-165">The privacy statement Url.</span></span> <span data-ttu-id="f61d2-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f61d2-167">informationUrl</span></span>|<span data-ttu-id="f61d2-168">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-168">String</span></span>|<span data-ttu-id="f61d2-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f61d2-169">The more information Url.</span></span> <span data-ttu-id="f61d2-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-171">owner</span><span class="sxs-lookup"><span data-stu-id="f61d2-171">owner</span></span>|<span data-ttu-id="f61d2-172">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-172">String</span></span>|<span data-ttu-id="f61d2-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-173">The owner of the app.</span></span> <span data-ttu-id="f61d2-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-175">developer</span><span class="sxs-lookup"><span data-stu-id="f61d2-175">developer</span></span>|<span data-ttu-id="f61d2-176">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-176">String</span></span>|<span data-ttu-id="f61d2-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-177">The developer of the app.</span></span> <span data-ttu-id="f61d2-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-179">notes</span><span class="sxs-lookup"><span data-stu-id="f61d2-179">notes</span></span>|<span data-ttu-id="f61d2-180">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-180">String</span></span>|<span data-ttu-id="f61d2-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="f61d2-181">Notes for the app.</span></span> <span data-ttu-id="f61d2-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f61d2-183">uploadState</span></span>|<span data-ttu-id="f61d2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f61d2-184">Int32</span></span>|<span data-ttu-id="f61d2-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f61d2-185">The upload state.</span></span> <span data-ttu-id="f61d2-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f61d2-187">publishingState</span></span>|[<span data-ttu-id="f61d2-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f61d2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f61d2-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-189">The publishing state for the app.</span></span> <span data-ttu-id="f61d2-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f61d2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f61d2-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f61d2-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f61d2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f61d2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f61d2-193">isAssigned</span></span>|<span data-ttu-id="f61d2-194">Логический</span><span class="sxs-lookup"><span data-stu-id="f61d2-194">Boolean</span></span>|<span data-ttu-id="f61d2-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="f61d2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f61d2-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f61d2-197">roleScopeTagIds</span></span>|<span data-ttu-id="f61d2-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f61d2-198">String collection</span></span>|<span data-ttu-id="f61d2-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f61d2-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f61d2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f61d2-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f61d2-201">usedLicenseCount</span></span>|<span data-ttu-id="f61d2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f61d2-202">Int32</span></span>|<span data-ttu-id="f61d2-203">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f61d2-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="f61d2-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f61d2-204">totalLicenseCount</span></span>|<span data-ttu-id="f61d2-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f61d2-205">Int32</span></span>|<span data-ttu-id="f61d2-206">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f61d2-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="f61d2-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="f61d2-207">releaseDateTime</span></span>|<span data-ttu-id="f61d2-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f61d2-208">DateTimeOffset</span></span>|<span data-ttu-id="f61d2-209">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="f61d2-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="f61d2-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f61d2-210">appStoreUrl</span></span>|<span data-ttu-id="f61d2-211">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-211">String</span></span>|<span data-ttu-id="f61d2-212">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="f61d2-212">The store URL.</span></span>|
|<span data-ttu-id="f61d2-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="f61d2-213">licensingType</span></span>|[<span data-ttu-id="f61d2-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f61d2-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="f61d2-215">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="f61d2-215">The supported License Type.</span></span>|
|<span data-ttu-id="f61d2-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f61d2-216">applicableDeviceType</span></span>|[<span data-ttu-id="f61d2-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f61d2-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f61d2-218">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="f61d2-218">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="f61d2-219">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f61d2-219">vppTokenOrganizationName</span></span>|<span data-ttu-id="f61d2-220">Строка</span><span class="sxs-lookup"><span data-stu-id="f61d2-220">String</span></span>|<span data-ttu-id="f61d2-221">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f61d2-221">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="f61d2-222">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f61d2-222">vppTokenAccountType</span></span>|[<span data-ttu-id="f61d2-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f61d2-223">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="f61d2-224">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f61d2-224">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="f61d2-225">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="f61d2-225">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="f61d2-226">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="f61d2-226">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="f61d2-227">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="f61d2-227">vppTokenAppleId</span></span>|<span data-ttu-id="f61d2-228">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-228">String</span></span>|<span data-ttu-id="f61d2-229">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f61d2-229">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f61d2-230">bundleId</span><span class="sxs-lookup"><span data-stu-id="f61d2-230">bundleId</span></span>|<span data-ttu-id="f61d2-231">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-231">String</span></span>|<span data-ttu-id="f61d2-232">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f61d2-232">The Identity Name.</span></span>|
|<span data-ttu-id="f61d2-233">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f61d2-233">vppTokenId</span></span>|<span data-ttu-id="f61d2-234">String</span><span class="sxs-lookup"><span data-stu-id="f61d2-234">String</span></span>|<span data-ttu-id="f61d2-235">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="f61d2-235">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="f61d2-236">Ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="f61d2-236">revokeLicenseActionResults</span></span>|<span data-ttu-id="f61d2-237">Коллекция [иосвппаппревокелиценсесактионресулт](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f61d2-237">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="f61d2-238">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="f61d2-238">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="f61d2-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="f61d2-239">Response</span></span>
<span data-ttu-id="f61d2-240">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f61d2-240">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f61d2-241">Пример</span><span class="sxs-lookup"><span data-stu-id="f61d2-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="f61d2-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="f61d2-242">Request</span></span>
<span data-ttu-id="f61d2-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f61d2-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1972

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

### <a name="response"></a><span data-ttu-id="f61d2-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="f61d2-244">Response</span></span>
<span data-ttu-id="f61d2-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f61d2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2144

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




