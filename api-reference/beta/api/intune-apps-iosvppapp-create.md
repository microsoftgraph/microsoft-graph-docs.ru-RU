---
title: Create iosVppApp
description: Создание объекта iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 992c2eef697c4ea9a7574ddab7870f75a2f90275
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700201"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="2726a-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="2726a-103">Create iosVppApp</span></span>

<span data-ttu-id="2726a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2726a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2726a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2726a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2726a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2726a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2726a-107">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2726a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2726a-108">Prerequisites</span></span>
<span data-ttu-id="2726a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2726a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2726a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2726a-111">Permission type</span></span>|<span data-ttu-id="2726a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2726a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2726a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2726a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2726a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2726a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2726a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2726a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2726a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2726a-116">Not supported.</span></span>|
|<span data-ttu-id="2726a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2726a-117">Application</span></span>|<span data-ttu-id="2726a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2726a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2726a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2726a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2726a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2726a-120">Request headers</span></span>
|<span data-ttu-id="2726a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2726a-121">Header</span></span>|<span data-ttu-id="2726a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2726a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2726a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2726a-123">Authorization</span></span>|<span data-ttu-id="2726a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2726a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2726a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2726a-125">Accept</span></span>|<span data-ttu-id="2726a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2726a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2726a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2726a-127">Request body</span></span>
<span data-ttu-id="2726a-128">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2726a-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="2726a-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="2726a-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="2726a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2726a-130">Property</span></span>|<span data-ttu-id="2726a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2726a-131">Type</span></span>|<span data-ttu-id="2726a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2726a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2726a-133">id</span><span class="sxs-lookup"><span data-stu-id="2726a-133">id</span></span>|<span data-ttu-id="2726a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2726a-134">String</span></span>|<span data-ttu-id="2726a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2726a-135">Key of the entity.</span></span> <span data-ttu-id="2726a-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2726a-137">displayName</span></span>|<span data-ttu-id="2726a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="2726a-138">String</span></span>|<span data-ttu-id="2726a-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2726a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2726a-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-141">description</span><span class="sxs-lookup"><span data-stu-id="2726a-141">description</span></span>|<span data-ttu-id="2726a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2726a-142">String</span></span>|<span data-ttu-id="2726a-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-143">The description of the app.</span></span> <span data-ttu-id="2726a-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2726a-145">publisher</span></span>|<span data-ttu-id="2726a-146">String</span><span class="sxs-lookup"><span data-stu-id="2726a-146">String</span></span>|<span data-ttu-id="2726a-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-147">The publisher of the app.</span></span> <span data-ttu-id="2726a-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2726a-149">largeIcon</span></span>|[<span data-ttu-id="2726a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2726a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2726a-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2726a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2726a-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2726a-153">createdDateTime</span></span>|<span data-ttu-id="2726a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2726a-154">DateTimeOffset</span></span>|<span data-ttu-id="2726a-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-155">The date and time the app was created.</span></span> <span data-ttu-id="2726a-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2726a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2726a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2726a-158">DateTimeOffset</span></span>|<span data-ttu-id="2726a-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2726a-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2726a-161">isFeatured</span></span>|<span data-ttu-id="2726a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2726a-162">Boolean</span></span>|<span data-ttu-id="2726a-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2726a-164">privacyInformationUrl</span></span>|<span data-ttu-id="2726a-165">String</span><span class="sxs-lookup"><span data-stu-id="2726a-165">String</span></span>|<span data-ttu-id="2726a-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2726a-166">The privacy statement Url.</span></span> <span data-ttu-id="2726a-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2726a-168">informationUrl</span></span>|<span data-ttu-id="2726a-169">String</span><span class="sxs-lookup"><span data-stu-id="2726a-169">String</span></span>|<span data-ttu-id="2726a-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2726a-170">The more information Url.</span></span> <span data-ttu-id="2726a-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-172">owner</span><span class="sxs-lookup"><span data-stu-id="2726a-172">owner</span></span>|<span data-ttu-id="2726a-173">String</span><span class="sxs-lookup"><span data-stu-id="2726a-173">String</span></span>|<span data-ttu-id="2726a-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-174">The owner of the app.</span></span> <span data-ttu-id="2726a-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-176">developer</span><span class="sxs-lookup"><span data-stu-id="2726a-176">developer</span></span>|<span data-ttu-id="2726a-177">String</span><span class="sxs-lookup"><span data-stu-id="2726a-177">String</span></span>|<span data-ttu-id="2726a-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-178">The developer of the app.</span></span> <span data-ttu-id="2726a-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-180">notes</span><span class="sxs-lookup"><span data-stu-id="2726a-180">notes</span></span>|<span data-ttu-id="2726a-181">String</span><span class="sxs-lookup"><span data-stu-id="2726a-181">String</span></span>|<span data-ttu-id="2726a-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-182">Notes for the app.</span></span> <span data-ttu-id="2726a-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2726a-184">uploadState</span></span>|<span data-ttu-id="2726a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2726a-185">Int32</span></span>|<span data-ttu-id="2726a-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="2726a-186">The upload state.</span></span> <span data-ttu-id="2726a-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="2726a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="2726a-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="2726a-189">publishingState</span></span>|[<span data-ttu-id="2726a-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="2726a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2726a-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-191">The publishing state for the app.</span></span> <span data-ttu-id="2726a-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2726a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2726a-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2726a-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2726a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2726a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2726a-195">isAssigned</span></span>|<span data-ttu-id="2726a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="2726a-196">Boolean</span></span>|<span data-ttu-id="2726a-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="2726a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2726a-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2726a-199">roleScopeTagIds</span></span>|<span data-ttu-id="2726a-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2726a-200">String collection</span></span>|<span data-ttu-id="2726a-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2726a-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2726a-203">dependentAppCount</span></span>|<span data-ttu-id="2726a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="2726a-204">Int32</span></span>|<span data-ttu-id="2726a-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="2726a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2726a-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2726a-207">supersedingAppCount</span></span>|<span data-ttu-id="2726a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="2726a-208">Int32</span></span>|<span data-ttu-id="2726a-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="2726a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="2726a-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2726a-211">supersededAppCount</span></span>|<span data-ttu-id="2726a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="2726a-212">Int32</span></span>|<span data-ttu-id="2726a-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="2726a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="2726a-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2726a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2726a-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2726a-215">usedLicenseCount</span></span>|<span data-ttu-id="2726a-216">Int32</span><span class="sxs-lookup"><span data-stu-id="2726a-216">Int32</span></span>|<span data-ttu-id="2726a-217">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2726a-217">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2726a-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2726a-218">totalLicenseCount</span></span>|<span data-ttu-id="2726a-219">Int32</span><span class="sxs-lookup"><span data-stu-id="2726a-219">Int32</span></span>|<span data-ttu-id="2726a-220">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2726a-220">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2726a-221">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="2726a-221">releaseDateTime</span></span>|<span data-ttu-id="2726a-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2726a-222">DateTimeOffset</span></span>|<span data-ttu-id="2726a-223">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="2726a-223">The VPP application release date and time.</span></span>|
|<span data-ttu-id="2726a-224">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2726a-224">appStoreUrl</span></span>|<span data-ttu-id="2726a-225">String</span><span class="sxs-lookup"><span data-stu-id="2726a-225">String</span></span>|<span data-ttu-id="2726a-226">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="2726a-226">The store URL.</span></span>|
|<span data-ttu-id="2726a-227">licensingType</span><span class="sxs-lookup"><span data-stu-id="2726a-227">licensingType</span></span>|[<span data-ttu-id="2726a-228">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2726a-228">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2726a-229">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="2726a-229">The supported License Type.</span></span>|
|<span data-ttu-id="2726a-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2726a-230">applicableDeviceType</span></span>|[<span data-ttu-id="2726a-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2726a-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2726a-232">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="2726a-232">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="2726a-233">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2726a-233">vppTokenOrganizationName</span></span>|<span data-ttu-id="2726a-234">String</span><span class="sxs-lookup"><span data-stu-id="2726a-234">String</span></span>|<span data-ttu-id="2726a-235">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2726a-235">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2726a-236">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2726a-236">vppTokenAccountType</span></span>|[<span data-ttu-id="2726a-237">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2726a-237">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2726a-238">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2726a-238">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2726a-239">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2726a-239">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2726a-240">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2726a-240">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2726a-241">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="2726a-241">vppTokenAppleId</span></span>|<span data-ttu-id="2726a-242">String</span><span class="sxs-lookup"><span data-stu-id="2726a-242">String</span></span>|<span data-ttu-id="2726a-243">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2726a-243">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2726a-244">bundleId</span><span class="sxs-lookup"><span data-stu-id="2726a-244">bundleId</span></span>|<span data-ttu-id="2726a-245">String</span><span class="sxs-lookup"><span data-stu-id="2726a-245">String</span></span>|<span data-ttu-id="2726a-246">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2726a-246">The Identity Name.</span></span>|
|<span data-ttu-id="2726a-247">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2726a-247">vppTokenId</span></span>|<span data-ttu-id="2726a-248">Строка</span><span class="sxs-lookup"><span data-stu-id="2726a-248">String</span></span>|<span data-ttu-id="2726a-249">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="2726a-249">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="2726a-250">ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="2726a-250">revokeLicenseActionResults</span></span>|<span data-ttu-id="2726a-251">Коллекция [иосвппаппревокелиценсесактионресулт](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2726a-251">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="2726a-252">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="2726a-252">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="2726a-253">Ответ</span><span class="sxs-lookup"><span data-stu-id="2726a-253">Response</span></span>
<span data-ttu-id="2726a-254">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2726a-254">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2726a-255">Пример</span><span class="sxs-lookup"><span data-stu-id="2726a-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="2726a-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="2726a-256">Request</span></span>
<span data-ttu-id="2726a-257">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2726a-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2056

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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

### <a name="response"></a><span data-ttu-id="2726a-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="2726a-258">Response</span></span>
<span data-ttu-id="2726a-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2726a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2228

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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





