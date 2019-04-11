---
title: Создание Макосвппапп
description: Создание нового объекта Макосвппапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53b526903b009748f9d926582e27dfd6b2f357a9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770671"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="b52e8-103">Создание Макосвппапп</span><span class="sxs-lookup"><span data-stu-id="b52e8-103">Create macOsVppApp</span></span>

> <span data-ttu-id="b52e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b52e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b52e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b52e8-106">Создание нового объекта [макосвппапп](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b52e8-106">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b52e8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b52e8-107">Prerequisites</span></span>
<span data-ttu-id="b52e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b52e8-110">Permission type</span></span>|<span data-ttu-id="b52e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b52e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b52e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b52e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b52e8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52e8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b52e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b52e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b52e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52e8-115">Not supported.</span></span>|
|<span data-ttu-id="b52e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b52e8-116">Application</span></span>|<span data-ttu-id="b52e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b52e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b52e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b52e8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b52e8-119">Request headers</span></span>
|<span data-ttu-id="b52e8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b52e8-120">Header</span></span>|<span data-ttu-id="b52e8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b52e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b52e8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b52e8-122">Authorization</span></span>|<span data-ttu-id="b52e8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b52e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b52e8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b52e8-124">Accept</span></span>|<span data-ttu-id="b52e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b52e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b52e8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b52e8-126">Request body</span></span>
<span data-ttu-id="b52e8-127">В тексте запроса добавьте представление объекта Макосвппапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b52e8-127">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="b52e8-128">В следующей таблице приведены свойства, необходимые при создании Макосвппапп.</span><span class="sxs-lookup"><span data-stu-id="b52e8-128">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="b52e8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b52e8-129">Property</span></span>|<span data-ttu-id="b52e8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b52e8-130">Type</span></span>|<span data-ttu-id="b52e8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b52e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b52e8-132">id</span><span class="sxs-lookup"><span data-stu-id="b52e8-132">id</span></span>|<span data-ttu-id="b52e8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b52e8-133">String</span></span>|<span data-ttu-id="b52e8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b52e8-134">Key of the entity.</span></span> <span data-ttu-id="b52e8-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b52e8-136">displayName</span></span>|<span data-ttu-id="b52e8-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b52e8-137">String</span></span>|<span data-ttu-id="b52e8-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b52e8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b52e8-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-140">description</span><span class="sxs-lookup"><span data-stu-id="b52e8-140">description</span></span>|<span data-ttu-id="b52e8-141">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-141">String</span></span>|<span data-ttu-id="b52e8-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-142">The description of the app.</span></span> <span data-ttu-id="b52e8-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b52e8-144">publisher</span></span>|<span data-ttu-id="b52e8-145">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-145">String</span></span>|<span data-ttu-id="b52e8-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-146">The publisher of the app.</span></span> <span data-ttu-id="b52e8-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b52e8-148">largeIcon</span></span>|[<span data-ttu-id="b52e8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b52e8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b52e8-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b52e8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b52e8-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b52e8-152">createdDateTime</span></span>|<span data-ttu-id="b52e8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52e8-153">DateTimeOffset</span></span>|<span data-ttu-id="b52e8-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-154">The date and time the app was created.</span></span> <span data-ttu-id="b52e8-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b52e8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b52e8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52e8-157">DateTimeOffset</span></span>|<span data-ttu-id="b52e8-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b52e8-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b52e8-160">isFeatured</span></span>|<span data-ttu-id="b52e8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b52e8-161">Boolean</span></span>|<span data-ttu-id="b52e8-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b52e8-163">privacyInformationUrl</span></span>|<span data-ttu-id="b52e8-164">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-164">String</span></span>|<span data-ttu-id="b52e8-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b52e8-165">The privacy statement Url.</span></span> <span data-ttu-id="b52e8-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b52e8-167">informationUrl</span></span>|<span data-ttu-id="b52e8-168">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-168">String</span></span>|<span data-ttu-id="b52e8-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b52e8-169">The more information Url.</span></span> <span data-ttu-id="b52e8-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-171">owner</span><span class="sxs-lookup"><span data-stu-id="b52e8-171">owner</span></span>|<span data-ttu-id="b52e8-172">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-172">String</span></span>|<span data-ttu-id="b52e8-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-173">The owner of the app.</span></span> <span data-ttu-id="b52e8-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-175">developer</span><span class="sxs-lookup"><span data-stu-id="b52e8-175">developer</span></span>|<span data-ttu-id="b52e8-176">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-176">String</span></span>|<span data-ttu-id="b52e8-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-177">The developer of the app.</span></span> <span data-ttu-id="b52e8-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-179">notes</span><span class="sxs-lookup"><span data-stu-id="b52e8-179">notes</span></span>|<span data-ttu-id="b52e8-180">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-180">String</span></span>|<span data-ttu-id="b52e8-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-181">Notes for the app.</span></span> <span data-ttu-id="b52e8-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b52e8-183">uploadState</span></span>|<span data-ttu-id="b52e8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b52e8-184">Int32</span></span>|<span data-ttu-id="b52e8-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b52e8-185">The upload state.</span></span> <span data-ttu-id="b52e8-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b52e8-187">publishingState</span></span>|[<span data-ttu-id="b52e8-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b52e8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b52e8-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-189">The publishing state for the app.</span></span> <span data-ttu-id="b52e8-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b52e8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b52e8-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b52e8-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b52e8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b52e8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b52e8-193">isAssigned</span></span>|<span data-ttu-id="b52e8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b52e8-194">Boolean</span></span>|<span data-ttu-id="b52e8-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b52e8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b52e8-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b52e8-197">roleScopeTagIds</span></span>|<span data-ttu-id="b52e8-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b52e8-198">String collection</span></span>|<span data-ttu-id="b52e8-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b52e8-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b52e8-201">dependentAppCount</span></span>|<span data-ttu-id="b52e8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b52e8-202">Int32</span></span>|<span data-ttu-id="b52e8-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b52e8-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b52e8-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b52e8-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b52e8-205">usedLicenseCount</span></span>|<span data-ttu-id="b52e8-206">Int32</span><span class="sxs-lookup"><span data-stu-id="b52e8-206">Int32</span></span>|<span data-ttu-id="b52e8-207">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="b52e8-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="b52e8-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b52e8-208">totalLicenseCount</span></span>|<span data-ttu-id="b52e8-209">Int32</span><span class="sxs-lookup"><span data-stu-id="b52e8-209">Int32</span></span>|<span data-ttu-id="b52e8-210">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="b52e8-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="b52e8-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b52e8-211">releaseDateTime</span></span>|<span data-ttu-id="b52e8-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b52e8-212">DateTimeOffset</span></span>|<span data-ttu-id="b52e8-213">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="b52e8-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="b52e8-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b52e8-214">appStoreUrl</span></span>|<span data-ttu-id="b52e8-215">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-215">String</span></span>|<span data-ttu-id="b52e8-216">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="b52e8-216">The store URL.</span></span>|
|<span data-ttu-id="b52e8-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="b52e8-217">licensingType</span></span>|[<span data-ttu-id="b52e8-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="b52e8-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="b52e8-219">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="b52e8-219">The supported License Type.</span></span>|
|<span data-ttu-id="b52e8-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b52e8-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="b52e8-221">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-221">String</span></span>|<span data-ttu-id="b52e8-222">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b52e8-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b52e8-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b52e8-223">vppTokenAccountType</span></span>|[<span data-ttu-id="b52e8-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b52e8-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="b52e8-225">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b52e8-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b52e8-226">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="b52e8-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="b52e8-227">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="b52e8-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b52e8-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="b52e8-228">vppTokenAppleId</span></span>|<span data-ttu-id="b52e8-229">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-229">String</span></span>|<span data-ttu-id="b52e8-230">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b52e8-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b52e8-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="b52e8-231">bundleId</span></span>|<span data-ttu-id="b52e8-232">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-232">String</span></span>|<span data-ttu-id="b52e8-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b52e8-233">The Identity Name.</span></span>|
|<span data-ttu-id="b52e8-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b52e8-234">vppTokenId</span></span>|<span data-ttu-id="b52e8-235">String</span><span class="sxs-lookup"><span data-stu-id="b52e8-235">String</span></span>|<span data-ttu-id="b52e8-236">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="b52e8-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="b52e8-237">Ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="b52e8-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="b52e8-238">Коллекция [макосвппаппревокелиценсесактионресулт](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b52e8-238">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="b52e8-239">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="b52e8-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="b52e8-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52e8-240">Response</span></span>
<span data-ttu-id="b52e8-241">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвппапп](../resources/intune-apps-macosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b52e8-241">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52e8-242">Пример</span><span class="sxs-lookup"><span data-stu-id="b52e8-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="b52e8-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="b52e8-243">Request</span></span>
<span data-ttu-id="b52e8-244">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b52e8-244">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b52e8-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52e8-245">Response</span></span>
<span data-ttu-id="b52e8-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b52e8-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





