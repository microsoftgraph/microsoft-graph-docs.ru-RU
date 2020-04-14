---
title: Create iosVppApp
description: Создание объекта iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3136e5ba079dbea1e876cf13245d8733b3952377
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394588"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="2b2cf-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="2b2cf-103">Create iosVppApp</span></span>

<span data-ttu-id="2b2cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b2cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b2cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b2cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b2cf-107">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b2cf-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2b2cf-108">Prerequisites</span></span>
<span data-ttu-id="2b2cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b2cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b2cf-111">Permission type</span></span>|<span data-ttu-id="2b2cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b2cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b2cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b2cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b2cf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b2cf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2b2cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b2cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b2cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-116">Not supported.</span></span>|
|<span data-ttu-id="2b2cf-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2b2cf-117">Application</span></span>|<span data-ttu-id="2b2cf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b2cf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b2cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b2cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2b2cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b2cf-120">Request headers</span></span>
|<span data-ttu-id="2b2cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b2cf-121">Header</span></span>|<span data-ttu-id="2b2cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b2cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b2cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b2cf-123">Authorization</span></span>|<span data-ttu-id="2b2cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b2cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b2cf-125">Accept</span></span>|<span data-ttu-id="2b2cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b2cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b2cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b2cf-127">Request body</span></span>
<span data-ttu-id="2b2cf-128">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="2b2cf-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="2b2cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b2cf-130">Property</span></span>|<span data-ttu-id="2b2cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b2cf-131">Type</span></span>|<span data-ttu-id="2b2cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b2cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b2cf-133">id</span><span class="sxs-lookup"><span data-stu-id="2b2cf-133">id</span></span>|<span data-ttu-id="2b2cf-134">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-134">String</span></span>|<span data-ttu-id="2b2cf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-135">Key of the entity.</span></span> <span data-ttu-id="2b2cf-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2b2cf-137">displayName</span></span>|<span data-ttu-id="2b2cf-138">Строка</span><span class="sxs-lookup"><span data-stu-id="2b2cf-138">String</span></span>|<span data-ttu-id="2b2cf-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2b2cf-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-141">description</span><span class="sxs-lookup"><span data-stu-id="2b2cf-141">description</span></span>|<span data-ttu-id="2b2cf-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2b2cf-142">String</span></span>|<span data-ttu-id="2b2cf-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-143">The description of the app.</span></span> <span data-ttu-id="2b2cf-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2b2cf-145">publisher</span></span>|<span data-ttu-id="2b2cf-146">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-146">String</span></span>|<span data-ttu-id="2b2cf-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-147">The publisher of the app.</span></span> <span data-ttu-id="2b2cf-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2b2cf-149">largeIcon</span></span>|[<span data-ttu-id="2b2cf-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2b2cf-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2b2cf-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2b2cf-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b2cf-153">createdDateTime</span></span>|<span data-ttu-id="2b2cf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b2cf-154">DateTimeOffset</span></span>|<span data-ttu-id="2b2cf-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-155">The date and time the app was created.</span></span> <span data-ttu-id="2b2cf-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b2cf-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2b2cf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b2cf-158">DateTimeOffset</span></span>|<span data-ttu-id="2b2cf-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2b2cf-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2b2cf-161">isFeatured</span></span>|<span data-ttu-id="2b2cf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b2cf-162">Boolean</span></span>|<span data-ttu-id="2b2cf-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2b2cf-164">privacyInformationUrl</span></span>|<span data-ttu-id="2b2cf-165">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-165">String</span></span>|<span data-ttu-id="2b2cf-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-166">The privacy statement Url.</span></span> <span data-ttu-id="2b2cf-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2b2cf-168">informationUrl</span></span>|<span data-ttu-id="2b2cf-169">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-169">String</span></span>|<span data-ttu-id="2b2cf-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-170">The more information Url.</span></span> <span data-ttu-id="2b2cf-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-172">owner</span><span class="sxs-lookup"><span data-stu-id="2b2cf-172">owner</span></span>|<span data-ttu-id="2b2cf-173">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-173">String</span></span>|<span data-ttu-id="2b2cf-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-174">The owner of the app.</span></span> <span data-ttu-id="2b2cf-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-176">developer</span><span class="sxs-lookup"><span data-stu-id="2b2cf-176">developer</span></span>|<span data-ttu-id="2b2cf-177">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-177">String</span></span>|<span data-ttu-id="2b2cf-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-178">The developer of the app.</span></span> <span data-ttu-id="2b2cf-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-180">notes</span><span class="sxs-lookup"><span data-stu-id="2b2cf-180">notes</span></span>|<span data-ttu-id="2b2cf-181">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-181">String</span></span>|<span data-ttu-id="2b2cf-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-182">Notes for the app.</span></span> <span data-ttu-id="2b2cf-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2b2cf-184">uploadState</span></span>|<span data-ttu-id="2b2cf-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2cf-185">Int32</span></span>|<span data-ttu-id="2b2cf-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-186">The upload state.</span></span> <span data-ttu-id="2b2cf-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2b2cf-188">publishingState</span></span>|[<span data-ttu-id="2b2cf-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="2b2cf-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2b2cf-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-190">The publishing state for the app.</span></span> <span data-ttu-id="2b2cf-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2b2cf-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2b2cf-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2b2cf-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2b2cf-194">isAssigned</span></span>|<span data-ttu-id="2b2cf-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b2cf-195">Boolean</span></span>|<span data-ttu-id="2b2cf-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2b2cf-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b2cf-198">roleScopeTagIds</span></span>|<span data-ttu-id="2b2cf-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-199">String collection</span></span>|<span data-ttu-id="2b2cf-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2b2cf-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2b2cf-202">dependentAppCount</span></span>|<span data-ttu-id="2b2cf-203">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2cf-203">Int32</span></span>|<span data-ttu-id="2b2cf-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2b2cf-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2b2cf-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2b2cf-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2b2cf-206">usedLicenseCount</span></span>|<span data-ttu-id="2b2cf-207">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2cf-207">Int32</span></span>|<span data-ttu-id="2b2cf-208">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2b2cf-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2b2cf-209">totalLicenseCount</span></span>|<span data-ttu-id="2b2cf-210">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2cf-210">Int32</span></span>|<span data-ttu-id="2b2cf-211">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2b2cf-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="2b2cf-212">releaseDateTime</span></span>|<span data-ttu-id="2b2cf-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b2cf-213">DateTimeOffset</span></span>|<span data-ttu-id="2b2cf-214">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="2b2cf-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2b2cf-215">appStoreUrl</span></span>|<span data-ttu-id="2b2cf-216">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-216">String</span></span>|<span data-ttu-id="2b2cf-217">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-217">The store URL.</span></span>|
|<span data-ttu-id="2b2cf-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="2b2cf-218">licensingType</span></span>|[<span data-ttu-id="2b2cf-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2b2cf-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2b2cf-220">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-220">The supported License Type.</span></span>|
|<span data-ttu-id="2b2cf-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2b2cf-221">applicableDeviceType</span></span>|[<span data-ttu-id="2b2cf-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2b2cf-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2b2cf-223">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-223">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="2b2cf-224">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2b2cf-224">vppTokenOrganizationName</span></span>|<span data-ttu-id="2b2cf-225">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-225">String</span></span>|<span data-ttu-id="2b2cf-226">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-226">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2b2cf-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2b2cf-227">vppTokenAccountType</span></span>|[<span data-ttu-id="2b2cf-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2b2cf-228">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2b2cf-229">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-229">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2b2cf-230">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-230">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2b2cf-231">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-231">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2b2cf-232">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="2b2cf-232">vppTokenAppleId</span></span>|<span data-ttu-id="2b2cf-233">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-233">String</span></span>|<span data-ttu-id="2b2cf-234">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-234">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2b2cf-235">bundleId</span><span class="sxs-lookup"><span data-stu-id="2b2cf-235">bundleId</span></span>|<span data-ttu-id="2b2cf-236">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-236">String</span></span>|<span data-ttu-id="2b2cf-237">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-237">The Identity Name.</span></span>|
|<span data-ttu-id="2b2cf-238">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2b2cf-238">vppTokenId</span></span>|<span data-ttu-id="2b2cf-239">String</span><span class="sxs-lookup"><span data-stu-id="2b2cf-239">String</span></span>|<span data-ttu-id="2b2cf-240">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-240">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="2b2cf-241">ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="2b2cf-241">revokeLicenseActionResults</span></span>|<span data-ttu-id="2b2cf-242">Коллекция [иосвппаппревокелиценсесактионресулт](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2b2cf-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="2b2cf-243">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-243">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="2b2cf-244">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b2cf-244">Response</span></span>
<span data-ttu-id="2b2cf-245">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-245">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b2cf-246">Пример</span><span class="sxs-lookup"><span data-stu-id="2b2cf-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b2cf-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b2cf-247">Request</span></span>
<span data-ttu-id="2b2cf-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b2cf-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b2cf-249">Response</span></span>
<span data-ttu-id="2b2cf-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b2cf-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



