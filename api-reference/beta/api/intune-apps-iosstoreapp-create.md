---
title: Create iosStoreApp
description: Создание объекта iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0eed3299a74db8c3dbb965cf13ee0e9f0157020a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495675"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="1c99f-103">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="1c99f-103">Create iosStoreApp</span></span>

> <span data-ttu-id="1c99f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c99f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c99f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c99f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c99f-106">Создание объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-106">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c99f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1c99f-107">Prerequisites</span></span>
<span data-ttu-id="1c99f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c99f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c99f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c99f-110">Permission type</span></span>|<span data-ttu-id="1c99f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c99f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c99f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c99f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c99f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c99f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c99f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c99f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c99f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c99f-115">Not supported.</span></span>|
|<span data-ttu-id="1c99f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c99f-116">Application</span></span>|<span data-ttu-id="1c99f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c99f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c99f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c99f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1c99f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c99f-119">Request headers</span></span>
|<span data-ttu-id="1c99f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c99f-120">Header</span></span>|<span data-ttu-id="1c99f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1c99f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c99f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c99f-122">Authorization</span></span>|<span data-ttu-id="1c99f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c99f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c99f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1c99f-124">Accept</span></span>|<span data-ttu-id="1c99f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c99f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c99f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c99f-126">Request body</span></span>
<span data-ttu-id="1c99f-127">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c99f-127">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="1c99f-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="1c99f-128">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="1c99f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c99f-129">Property</span></span>|<span data-ttu-id="1c99f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1c99f-130">Type</span></span>|<span data-ttu-id="1c99f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1c99f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c99f-132">id</span><span class="sxs-lookup"><span data-stu-id="1c99f-132">id</span></span>|<span data-ttu-id="1c99f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1c99f-133">String</span></span>|<span data-ttu-id="1c99f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c99f-134">Key of the entity.</span></span> <span data-ttu-id="1c99f-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1c99f-136">displayName</span></span>|<span data-ttu-id="1c99f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1c99f-137">String</span></span>|<span data-ttu-id="1c99f-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1c99f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1c99f-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-140">description</span><span class="sxs-lookup"><span data-stu-id="1c99f-140">description</span></span>|<span data-ttu-id="1c99f-141">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-141">String</span></span>|<span data-ttu-id="1c99f-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-142">The description of the app.</span></span> <span data-ttu-id="1c99f-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1c99f-144">publisher</span></span>|<span data-ttu-id="1c99f-145">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-145">String</span></span>|<span data-ttu-id="1c99f-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-146">The publisher of the app.</span></span> <span data-ttu-id="1c99f-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1c99f-148">largeIcon</span></span>|[<span data-ttu-id="1c99f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1c99f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1c99f-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1c99f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1c99f-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c99f-152">createdDateTime</span></span>|<span data-ttu-id="1c99f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c99f-153">DateTimeOffset</span></span>|<span data-ttu-id="1c99f-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-154">The date and time the app was created.</span></span> <span data-ttu-id="1c99f-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c99f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1c99f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c99f-157">DateTimeOffset</span></span>|<span data-ttu-id="1c99f-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1c99f-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1c99f-160">isFeatured</span></span>|<span data-ttu-id="1c99f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c99f-161">Boolean</span></span>|<span data-ttu-id="1c99f-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1c99f-163">privacyInformationUrl</span></span>|<span data-ttu-id="1c99f-164">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-164">String</span></span>|<span data-ttu-id="1c99f-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1c99f-165">The privacy statement Url.</span></span> <span data-ttu-id="1c99f-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1c99f-167">informationUrl</span></span>|<span data-ttu-id="1c99f-168">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-168">String</span></span>|<span data-ttu-id="1c99f-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1c99f-169">The more information Url.</span></span> <span data-ttu-id="1c99f-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-171">owner</span><span class="sxs-lookup"><span data-stu-id="1c99f-171">owner</span></span>|<span data-ttu-id="1c99f-172">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-172">String</span></span>|<span data-ttu-id="1c99f-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-173">The owner of the app.</span></span> <span data-ttu-id="1c99f-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-175">developer</span><span class="sxs-lookup"><span data-stu-id="1c99f-175">developer</span></span>|<span data-ttu-id="1c99f-176">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-176">String</span></span>|<span data-ttu-id="1c99f-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-177">The developer of the app.</span></span> <span data-ttu-id="1c99f-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-179">notes</span><span class="sxs-lookup"><span data-stu-id="1c99f-179">notes</span></span>|<span data-ttu-id="1c99f-180">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-180">String</span></span>|<span data-ttu-id="1c99f-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-181">Notes for the app.</span></span> <span data-ttu-id="1c99f-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1c99f-183">uploadState</span></span>|<span data-ttu-id="1c99f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1c99f-184">Int32</span></span>|<span data-ttu-id="1c99f-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="1c99f-185">The upload state.</span></span> <span data-ttu-id="1c99f-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1c99f-187">publishingState</span></span>|[<span data-ttu-id="1c99f-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1c99f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1c99f-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-189">The publishing state for the app.</span></span> <span data-ttu-id="1c99f-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1c99f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1c99f-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1c99f-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1c99f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1c99f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1c99f-193">isAssigned</span></span>|<span data-ttu-id="1c99f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c99f-194">Boolean</span></span>|<span data-ttu-id="1c99f-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="1c99f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1c99f-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c99f-197">roleScopeTagIds</span></span>|<span data-ttu-id="1c99f-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1c99f-198">String collection</span></span>|<span data-ttu-id="1c99f-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1c99f-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1c99f-201">dependentAppCount</span></span>|<span data-ttu-id="1c99f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="1c99f-202">Int32</span></span>|<span data-ttu-id="1c99f-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1c99f-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c99f-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c99f-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="1c99f-205">bundleId</span></span>|<span data-ttu-id="1c99f-206">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-206">String</span></span>|<span data-ttu-id="1c99f-207">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="1c99f-207">The Identity Name.</span></span>|
|<span data-ttu-id="1c99f-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1c99f-208">appStoreUrl</span></span>|<span data-ttu-id="1c99f-209">String</span><span class="sxs-lookup"><span data-stu-id="1c99f-209">String</span></span>|<span data-ttu-id="1c99f-210">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="1c99f-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="1c99f-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1c99f-211">applicableDeviceType</span></span>|[<span data-ttu-id="1c99f-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1c99f-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1c99f-213">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="1c99f-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1c99f-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1c99f-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1c99f-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1c99f-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1c99f-216">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="1c99f-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1c99f-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c99f-217">Response</span></span>
<span data-ttu-id="1c99f-218">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c99f-218">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c99f-219">Пример</span><span class="sxs-lookup"><span data-stu-id="1c99f-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c99f-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c99f-220">Request</span></span>
<span data-ttu-id="1c99f-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c99f-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="1c99f-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c99f-222">Response</span></span>
<span data-ttu-id="1c99f-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c99f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1312

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```





