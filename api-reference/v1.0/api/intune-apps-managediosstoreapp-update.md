---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c4f4d8c24acab38ecef0ec1df1ea40642f64b64
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516140"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="cf1c0-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="cf1c0-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="cf1c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf1c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf1c0-106">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf1c0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf1c0-107">Prerequisites</span></span>
<span data-ttu-id="cf1c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf1c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf1c0-110">Permission type</span></span>|<span data-ttu-id="cf1c0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf1c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf1c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf1c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf1c0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf1c0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf1c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf1c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf1c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-115">Not supported.</span></span>|
|<span data-ttu-id="cf1c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf1c0-116">Application</span></span>|<span data-ttu-id="cf1c0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf1c0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf1c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf1c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cf1c0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cf1c0-119">Request headers</span></span>
|<span data-ttu-id="cf1c0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf1c0-120">Header</span></span>|<span data-ttu-id="cf1c0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cf1c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf1c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf1c0-122">Authorization</span></span>|<span data-ttu-id="cf1c0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf1c0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cf1c0-124">Accept</span></span>|<span data-ttu-id="cf1c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf1c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf1c0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf1c0-126">Request body</span></span>
<span data-ttu-id="cf1c0-127">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="cf1c0-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="cf1c0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf1c0-129">Property</span></span>|<span data-ttu-id="cf1c0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cf1c0-130">Type</span></span>|<span data-ttu-id="cf1c0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cf1c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf1c0-132">id</span><span class="sxs-lookup"><span data-stu-id="cf1c0-132">id</span></span>|<span data-ttu-id="cf1c0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-133">String</span></span>|<span data-ttu-id="cf1c0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-134">Key of the entity.</span></span> <span data-ttu-id="cf1c0-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cf1c0-136">displayName</span></span>|<span data-ttu-id="cf1c0-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-137">String</span></span>|<span data-ttu-id="cf1c0-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cf1c0-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-140">description</span><span class="sxs-lookup"><span data-stu-id="cf1c0-140">description</span></span>|<span data-ttu-id="cf1c0-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-141">String</span></span>|<span data-ttu-id="cf1c0-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-142">The description of the app.</span></span> <span data-ttu-id="cf1c0-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cf1c0-144">publisher</span></span>|<span data-ttu-id="cf1c0-145">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-145">String</span></span>|<span data-ttu-id="cf1c0-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-146">The publisher of the app.</span></span> <span data-ttu-id="cf1c0-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cf1c0-148">largeIcon</span></span>|[<span data-ttu-id="cf1c0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cf1c0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cf1c0-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cf1c0-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf1c0-152">createdDateTime</span></span>|<span data-ttu-id="cf1c0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf1c0-153">DateTimeOffset</span></span>|<span data-ttu-id="cf1c0-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-154">The date and time the app was created.</span></span> <span data-ttu-id="cf1c0-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf1c0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cf1c0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf1c0-157">DateTimeOffset</span></span>|<span data-ttu-id="cf1c0-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cf1c0-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cf1c0-160">isFeatured</span></span>|<span data-ttu-id="cf1c0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf1c0-161">Boolean</span></span>|<span data-ttu-id="cf1c0-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cf1c0-163">privacyInformationUrl</span></span>|<span data-ttu-id="cf1c0-164">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-164">String</span></span>|<span data-ttu-id="cf1c0-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-165">The privacy statement Url.</span></span> <span data-ttu-id="cf1c0-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cf1c0-167">informationUrl</span></span>|<span data-ttu-id="cf1c0-168">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-168">String</span></span>|<span data-ttu-id="cf1c0-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-169">The more information Url.</span></span> <span data-ttu-id="cf1c0-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-171">owner</span><span class="sxs-lookup"><span data-stu-id="cf1c0-171">owner</span></span>|<span data-ttu-id="cf1c0-172">String</span><span class="sxs-lookup"><span data-stu-id="cf1c0-172">String</span></span>|<span data-ttu-id="cf1c0-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-173">The owner of the app.</span></span> <span data-ttu-id="cf1c0-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-175">developer</span><span class="sxs-lookup"><span data-stu-id="cf1c0-175">developer</span></span>|<span data-ttu-id="cf1c0-176">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-176">String</span></span>|<span data-ttu-id="cf1c0-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-177">The developer of the app.</span></span> <span data-ttu-id="cf1c0-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-179">notes</span><span class="sxs-lookup"><span data-stu-id="cf1c0-179">notes</span></span>|<span data-ttu-id="cf1c0-180">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-180">String</span></span>|<span data-ttu-id="cf1c0-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-181">Notes for the app.</span></span> <span data-ttu-id="cf1c0-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cf1c0-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="cf1c0-183">publishingState</span></span>|[<span data-ttu-id="cf1c0-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="cf1c0-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cf1c0-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-185">The publishing state for the app.</span></span> <span data-ttu-id="cf1c0-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cf1c0-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cf1c0-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cf1c0-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cf1c0-189">appAvailability</span></span>|[<span data-ttu-id="cf1c0-190">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="cf1c0-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cf1c0-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-191">The Application's availability.</span></span> <span data-ttu-id="cf1c0-192">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cf1c0-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cf1c0-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cf1c0-194">version</span><span class="sxs-lookup"><span data-stu-id="cf1c0-194">version</span></span>|<span data-ttu-id="cf1c0-195">String</span><span class="sxs-lookup"><span data-stu-id="cf1c0-195">String</span></span>|<span data-ttu-id="cf1c0-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-196">The Application's version.</span></span> <span data-ttu-id="cf1c0-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cf1c0-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cf1c0-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="cf1c0-198">bundleId</span></span>|<span data-ttu-id="cf1c0-199">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1c0-199">String</span></span>|<span data-ttu-id="cf1c0-200">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="cf1c0-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cf1c0-201">appStoreUrl</span></span>|<span data-ttu-id="cf1c0-202">String</span><span class="sxs-lookup"><span data-stu-id="cf1c0-202">String</span></span>|<span data-ttu-id="cf1c0-203">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="cf1c0-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cf1c0-204">applicableDeviceType</span></span>|[<span data-ttu-id="cf1c0-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cf1c0-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="cf1c0-206">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cf1c0-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cf1c0-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cf1c0-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cf1c0-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="cf1c0-209">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="cf1c0-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf1c0-210">Response</span></span>
<span data-ttu-id="cf1c0-211">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-211">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf1c0-212">Пример</span><span class="sxs-lookup"><span data-stu-id="cf1c0-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf1c0-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf1c0-213">Request</span></span>
<span data-ttu-id="cf1c0-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1104

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="cf1c0-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf1c0-215">Response</span></span>
<span data-ttu-id="cf1c0-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf1c0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1276

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v12_0": true,
    "v13_0": true
  }
}
```




