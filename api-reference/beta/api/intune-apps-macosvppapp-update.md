---
title: Обновление Макосвппапп
description: Обновление свойств объекта Макосвппапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cfd68791f3d5b7b930965b7d0f5d5eb7e54eac5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149100"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="2ab51-103">Обновление Макосвппапп</span><span class="sxs-lookup"><span data-stu-id="2ab51-103">Update macOsVppApp</span></span>

> <span data-ttu-id="2ab51-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ab51-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ab51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ab51-106">Обновление свойств объекта [макосвппапп](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2ab51-106">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ab51-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ab51-107">Prerequisites</span></span>
<span data-ttu-id="2ab51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ab51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ab51-110">Permission type</span></span>|<span data-ttu-id="2ab51-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ab51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ab51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab51-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ab51-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ab51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ab51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab51-115">Not supported.</span></span>|
|<span data-ttu-id="2ab51-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ab51-116">Application</span></span>|<span data-ttu-id="2ab51-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ab51-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab51-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ab51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2ab51-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ab51-119">Request headers</span></span>
|<span data-ttu-id="2ab51-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ab51-120">Header</span></span>|<span data-ttu-id="2ab51-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2ab51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab51-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ab51-122">Authorization</span></span>|<span data-ttu-id="2ab51-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2ab51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab51-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2ab51-124">Accept</span></span>|<span data-ttu-id="2ab51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab51-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ab51-126">Request body</span></span>
<span data-ttu-id="2ab51-127">В тексте запроса добавьте представление объекта [Макосвппапп](../resources/intune-apps-macosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ab51-127">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="2ab51-128">В следующей таблице приведены свойства, необходимые при создании [макосвппапп](../resources/intune-apps-macosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-128">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="2ab51-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ab51-129">Property</span></span>|<span data-ttu-id="2ab51-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2ab51-130">Type</span></span>|<span data-ttu-id="2ab51-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab51-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab51-132">id</span><span class="sxs-lookup"><span data-stu-id="2ab51-132">id</span></span>|<span data-ttu-id="2ab51-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab51-133">String</span></span>|<span data-ttu-id="2ab51-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2ab51-134">Key of the entity.</span></span> <span data-ttu-id="2ab51-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2ab51-136">displayName</span></span>|<span data-ttu-id="2ab51-137">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-137">String</span></span>|<span data-ttu-id="2ab51-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2ab51-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2ab51-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-140">description</span><span class="sxs-lookup"><span data-stu-id="2ab51-140">description</span></span>|<span data-ttu-id="2ab51-141">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab51-141">String</span></span>|<span data-ttu-id="2ab51-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-142">The description of the app.</span></span> <span data-ttu-id="2ab51-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2ab51-144">publisher</span></span>|<span data-ttu-id="2ab51-145">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-145">String</span></span>|<span data-ttu-id="2ab51-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-146">The publisher of the app.</span></span> <span data-ttu-id="2ab51-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2ab51-148">largeIcon</span></span>|[<span data-ttu-id="2ab51-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2ab51-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2ab51-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2ab51-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2ab51-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab51-152">createdDateTime</span></span>|<span data-ttu-id="2ab51-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab51-153">DateTimeOffset</span></span>|<span data-ttu-id="2ab51-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-154">The date and time the app was created.</span></span> <span data-ttu-id="2ab51-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab51-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2ab51-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab51-157">DateTimeOffset</span></span>|<span data-ttu-id="2ab51-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2ab51-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2ab51-160">isFeatured</span></span>|<span data-ttu-id="2ab51-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ab51-161">Boolean</span></span>|<span data-ttu-id="2ab51-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2ab51-163">privacyInformationUrl</span></span>|<span data-ttu-id="2ab51-164">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-164">String</span></span>|<span data-ttu-id="2ab51-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2ab51-165">The privacy statement Url.</span></span> <span data-ttu-id="2ab51-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2ab51-167">informationUrl</span></span>|<span data-ttu-id="2ab51-168">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-168">String</span></span>|<span data-ttu-id="2ab51-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2ab51-169">The more information Url.</span></span> <span data-ttu-id="2ab51-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-171">owner</span><span class="sxs-lookup"><span data-stu-id="2ab51-171">owner</span></span>|<span data-ttu-id="2ab51-172">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-172">String</span></span>|<span data-ttu-id="2ab51-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-173">The owner of the app.</span></span> <span data-ttu-id="2ab51-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-175">developer</span><span class="sxs-lookup"><span data-stu-id="2ab51-175">developer</span></span>|<span data-ttu-id="2ab51-176">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-176">String</span></span>|<span data-ttu-id="2ab51-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-177">The developer of the app.</span></span> <span data-ttu-id="2ab51-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-179">notes</span><span class="sxs-lookup"><span data-stu-id="2ab51-179">notes</span></span>|<span data-ttu-id="2ab51-180">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-180">String</span></span>|<span data-ttu-id="2ab51-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="2ab51-181">Notes for the app.</span></span> <span data-ttu-id="2ab51-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2ab51-183">uploadState</span></span>|<span data-ttu-id="2ab51-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab51-184">Int32</span></span>|<span data-ttu-id="2ab51-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="2ab51-185">The upload state.</span></span> <span data-ttu-id="2ab51-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2ab51-187">publishingState</span></span>|[<span data-ttu-id="2ab51-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="2ab51-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2ab51-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-189">The publishing state for the app.</span></span> <span data-ttu-id="2ab51-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2ab51-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2ab51-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2ab51-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2ab51-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2ab51-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2ab51-193">isAssigned</span></span>|<span data-ttu-id="2ab51-194">Логический</span><span class="sxs-lookup"><span data-stu-id="2ab51-194">Boolean</span></span>|<span data-ttu-id="2ab51-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="2ab51-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2ab51-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ab51-197">roleScopeTagIds</span></span>|<span data-ttu-id="2ab51-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ab51-198">String collection</span></span>|<span data-ttu-id="2ab51-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2ab51-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ab51-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2ab51-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2ab51-201">usedLicenseCount</span></span>|<span data-ttu-id="2ab51-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab51-202">Int32</span></span>|<span data-ttu-id="2ab51-203">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2ab51-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2ab51-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2ab51-204">totalLicenseCount</span></span>|<span data-ttu-id="2ab51-205">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab51-205">Int32</span></span>|<span data-ttu-id="2ab51-206">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2ab51-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2ab51-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="2ab51-207">releaseDateTime</span></span>|<span data-ttu-id="2ab51-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ab51-208">DateTimeOffset</span></span>|<span data-ttu-id="2ab51-209">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="2ab51-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="2ab51-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2ab51-210">appStoreUrl</span></span>|<span data-ttu-id="2ab51-211">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-211">String</span></span>|<span data-ttu-id="2ab51-212">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="2ab51-212">The store URL.</span></span>|
|<span data-ttu-id="2ab51-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="2ab51-213">licensingType</span></span>|[<span data-ttu-id="2ab51-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2ab51-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2ab51-215">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="2ab51-215">The supported License Type.</span></span>|
|<span data-ttu-id="2ab51-216">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2ab51-216">vppTokenOrganizationName</span></span>|<span data-ttu-id="2ab51-217">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab51-217">String</span></span>|<span data-ttu-id="2ab51-218">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2ab51-218">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2ab51-219">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2ab51-219">vppTokenAccountType</span></span>|[<span data-ttu-id="2ab51-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2ab51-220">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2ab51-221">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2ab51-221">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2ab51-222">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2ab51-222">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2ab51-223">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2ab51-223">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2ab51-224">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="2ab51-224">vppTokenAppleId</span></span>|<span data-ttu-id="2ab51-225">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-225">String</span></span>|<span data-ttu-id="2ab51-226">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2ab51-226">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2ab51-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="2ab51-227">bundleId</span></span>|<span data-ttu-id="2ab51-228">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-228">String</span></span>|<span data-ttu-id="2ab51-229">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2ab51-229">The Identity Name.</span></span>|
|<span data-ttu-id="2ab51-230">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2ab51-230">vppTokenId</span></span>|<span data-ttu-id="2ab51-231">String</span><span class="sxs-lookup"><span data-stu-id="2ab51-231">String</span></span>|<span data-ttu-id="2ab51-232">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="2ab51-232">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="2ab51-233">Ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="2ab51-233">revokeLicenseActionResults</span></span>|<span data-ttu-id="2ab51-234">Коллекция [макосвппаппревокелиценсесактионресулт](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2ab51-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="2ab51-235">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="2ab51-235">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="2ab51-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ab51-236">Response</span></span>
<span data-ttu-id="2ab51-237">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвппапп](../resources/intune-apps-macosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ab51-237">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab51-238">Пример</span><span class="sxs-lookup"><span data-stu-id="2ab51-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ab51-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ab51-239">Request</span></span>
<span data-ttu-id="2ab51-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ab51-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="2ab51-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ab51-241">Response</span></span>
<span data-ttu-id="2ab51-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ab51-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




