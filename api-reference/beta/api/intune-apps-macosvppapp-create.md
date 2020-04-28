---
title: Создание Макосвппапп
description: Создание нового объекта Макосвппапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0d0704c6c4fca4411656dcbf604fde85004d7af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409965"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="ff071-103">Создание Макосвппапп</span><span class="sxs-lookup"><span data-stu-id="ff071-103">Create macOsVppApp</span></span>

<span data-ttu-id="ff071-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff071-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff071-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff071-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff071-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff071-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff071-107">Создание нового объекта [макосвппапп](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ff071-107">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff071-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff071-108">Prerequisites</span></span>
<span data-ttu-id="ff071-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff071-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff071-111">Permission type</span></span>|<span data-ttu-id="ff071-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff071-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff071-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff071-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff071-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff071-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff071-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff071-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff071-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff071-116">Not supported.</span></span>|
|<span data-ttu-id="ff071-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff071-117">Application</span></span>|<span data-ttu-id="ff071-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff071-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff071-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff071-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ff071-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff071-120">Request headers</span></span>
|<span data-ttu-id="ff071-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff071-121">Header</span></span>|<span data-ttu-id="ff071-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff071-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff071-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff071-123">Authorization</span></span>|<span data-ttu-id="ff071-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff071-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff071-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff071-125">Accept</span></span>|<span data-ttu-id="ff071-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff071-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff071-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff071-127">Request body</span></span>
<span data-ttu-id="ff071-128">В тексте запроса добавьте представление объекта Макосвппапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff071-128">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="ff071-129">В следующей таблице приведены свойства, необходимые при создании Макосвппапп.</span><span class="sxs-lookup"><span data-stu-id="ff071-129">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="ff071-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff071-130">Property</span></span>|<span data-ttu-id="ff071-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff071-131">Type</span></span>|<span data-ttu-id="ff071-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff071-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff071-133">id</span><span class="sxs-lookup"><span data-stu-id="ff071-133">id</span></span>|<span data-ttu-id="ff071-134">String</span><span class="sxs-lookup"><span data-stu-id="ff071-134">String</span></span>|<span data-ttu-id="ff071-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff071-135">Key of the entity.</span></span> <span data-ttu-id="ff071-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ff071-137">displayName</span></span>|<span data-ttu-id="ff071-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ff071-138">String</span></span>|<span data-ttu-id="ff071-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ff071-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ff071-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-141">description</span><span class="sxs-lookup"><span data-stu-id="ff071-141">description</span></span>|<span data-ttu-id="ff071-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ff071-142">String</span></span>|<span data-ttu-id="ff071-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-143">The description of the app.</span></span> <span data-ttu-id="ff071-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ff071-145">publisher</span></span>|<span data-ttu-id="ff071-146">String</span><span class="sxs-lookup"><span data-stu-id="ff071-146">String</span></span>|<span data-ttu-id="ff071-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-147">The publisher of the app.</span></span> <span data-ttu-id="ff071-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ff071-149">largeIcon</span></span>|[<span data-ttu-id="ff071-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff071-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff071-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ff071-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ff071-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff071-153">createdDateTime</span></span>|<span data-ttu-id="ff071-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff071-154">DateTimeOffset</span></span>|<span data-ttu-id="ff071-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-155">The date and time the app was created.</span></span> <span data-ttu-id="ff071-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff071-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ff071-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff071-158">DateTimeOffset</span></span>|<span data-ttu-id="ff071-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ff071-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ff071-161">isFeatured</span></span>|<span data-ttu-id="ff071-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff071-162">Boolean</span></span>|<span data-ttu-id="ff071-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff071-164">privacyInformationUrl</span></span>|<span data-ttu-id="ff071-165">String</span><span class="sxs-lookup"><span data-stu-id="ff071-165">String</span></span>|<span data-ttu-id="ff071-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ff071-166">The privacy statement Url.</span></span> <span data-ttu-id="ff071-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff071-168">informationUrl</span></span>|<span data-ttu-id="ff071-169">String</span><span class="sxs-lookup"><span data-stu-id="ff071-169">String</span></span>|<span data-ttu-id="ff071-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ff071-170">The more information Url.</span></span> <span data-ttu-id="ff071-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-172">owner</span><span class="sxs-lookup"><span data-stu-id="ff071-172">owner</span></span>|<span data-ttu-id="ff071-173">String</span><span class="sxs-lookup"><span data-stu-id="ff071-173">String</span></span>|<span data-ttu-id="ff071-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-174">The owner of the app.</span></span> <span data-ttu-id="ff071-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-176">developer</span><span class="sxs-lookup"><span data-stu-id="ff071-176">developer</span></span>|<span data-ttu-id="ff071-177">String</span><span class="sxs-lookup"><span data-stu-id="ff071-177">String</span></span>|<span data-ttu-id="ff071-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-178">The developer of the app.</span></span> <span data-ttu-id="ff071-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-180">notes</span><span class="sxs-lookup"><span data-stu-id="ff071-180">notes</span></span>|<span data-ttu-id="ff071-181">String</span><span class="sxs-lookup"><span data-stu-id="ff071-181">String</span></span>|<span data-ttu-id="ff071-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-182">Notes for the app.</span></span> <span data-ttu-id="ff071-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ff071-184">uploadState</span></span>|<span data-ttu-id="ff071-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ff071-185">Int32</span></span>|<span data-ttu-id="ff071-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ff071-186">The upload state.</span></span> <span data-ttu-id="ff071-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ff071-188">publishingState</span></span>|[<span data-ttu-id="ff071-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="ff071-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ff071-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-190">The publishing state for the app.</span></span> <span data-ttu-id="ff071-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ff071-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ff071-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ff071-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ff071-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ff071-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ff071-194">isAssigned</span></span>|<span data-ttu-id="ff071-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff071-195">Boolean</span></span>|<span data-ttu-id="ff071-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="ff071-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ff071-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff071-198">roleScopeTagIds</span></span>|<span data-ttu-id="ff071-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ff071-199">String collection</span></span>|<span data-ttu-id="ff071-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ff071-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ff071-202">dependentAppCount</span></span>|<span data-ttu-id="ff071-203">Int32</span><span class="sxs-lookup"><span data-stu-id="ff071-203">Int32</span></span>|<span data-ttu-id="ff071-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="ff071-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ff071-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff071-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff071-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff071-206">usedLicenseCount</span></span>|<span data-ttu-id="ff071-207">Int32</span><span class="sxs-lookup"><span data-stu-id="ff071-207">Int32</span></span>|<span data-ttu-id="ff071-208">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="ff071-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="ff071-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff071-209">totalLicenseCount</span></span>|<span data-ttu-id="ff071-210">Int32</span><span class="sxs-lookup"><span data-stu-id="ff071-210">Int32</span></span>|<span data-ttu-id="ff071-211">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="ff071-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="ff071-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ff071-212">releaseDateTime</span></span>|<span data-ttu-id="ff071-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff071-213">DateTimeOffset</span></span>|<span data-ttu-id="ff071-214">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="ff071-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="ff071-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ff071-215">appStoreUrl</span></span>|<span data-ttu-id="ff071-216">String</span><span class="sxs-lookup"><span data-stu-id="ff071-216">String</span></span>|<span data-ttu-id="ff071-217">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="ff071-217">The store URL.</span></span>|
|<span data-ttu-id="ff071-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="ff071-218">licensingType</span></span>|[<span data-ttu-id="ff071-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="ff071-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="ff071-220">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="ff071-220">The supported License Type.</span></span>|
|<span data-ttu-id="ff071-221">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ff071-221">vppTokenOrganizationName</span></span>|<span data-ttu-id="ff071-222">String</span><span class="sxs-lookup"><span data-stu-id="ff071-222">String</span></span>|<span data-ttu-id="ff071-223">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ff071-223">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ff071-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ff071-224">vppTokenAccountType</span></span>|[<span data-ttu-id="ff071-225">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ff071-225">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ff071-226">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ff071-226">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ff071-227">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ff071-227">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ff071-228">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ff071-228">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ff071-229">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="ff071-229">vppTokenAppleId</span></span>|<span data-ttu-id="ff071-230">String</span><span class="sxs-lookup"><span data-stu-id="ff071-230">String</span></span>|<span data-ttu-id="ff071-231">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ff071-231">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ff071-232">bundleId</span><span class="sxs-lookup"><span data-stu-id="ff071-232">bundleId</span></span>|<span data-ttu-id="ff071-233">String</span><span class="sxs-lookup"><span data-stu-id="ff071-233">String</span></span>|<span data-ttu-id="ff071-234">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ff071-234">The Identity Name.</span></span>|
|<span data-ttu-id="ff071-235">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ff071-235">vppTokenId</span></span>|<span data-ttu-id="ff071-236">String</span><span class="sxs-lookup"><span data-stu-id="ff071-236">String</span></span>|<span data-ttu-id="ff071-237">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ff071-237">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="ff071-238">ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="ff071-238">revokeLicenseActionResults</span></span>|<span data-ttu-id="ff071-239">Коллекция [макосвппаппревокелиценсесактионресулт](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff071-239">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="ff071-240">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="ff071-240">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="ff071-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff071-241">Response</span></span>
<span data-ttu-id="ff071-242">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвппапп](../resources/intune-apps-macosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff071-242">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff071-243">Пример</span><span class="sxs-lookup"><span data-stu-id="ff071-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff071-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff071-244">Request</span></span>
<span data-ttu-id="ff071-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff071-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1869

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

### <a name="response"></a><span data-ttu-id="ff071-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff071-246">Response</span></span>
<span data-ttu-id="ff071-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff071-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2041

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



