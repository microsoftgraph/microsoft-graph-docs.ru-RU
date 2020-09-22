---
title: Create managedIOSStoreApp
description: Создание объекта managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f8d2748e3ea1c2b57a7e9906ae8d3bea11dcfec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997461"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="9a6de-103">Create managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="9a6de-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="9a6de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a6de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a6de-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a6de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a6de-106">Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a6de-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9a6de-107">Prerequisites</span></span>
<span data-ttu-id="9a6de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9a6de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a6de-110">Permission type</span></span>|<span data-ttu-id="9a6de-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a6de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a6de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a6de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a6de-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6de-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9a6de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a6de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a6de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a6de-115">Not supported.</span></span>|
|<span data-ttu-id="9a6de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a6de-116">Application</span></span>|<span data-ttu-id="9a6de-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a6de-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a6de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a6de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9a6de-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a6de-119">Request headers</span></span>
|<span data-ttu-id="9a6de-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a6de-120">Header</span></span>|<span data-ttu-id="9a6de-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9a6de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a6de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a6de-122">Authorization</span></span>|<span data-ttu-id="9a6de-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a6de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a6de-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9a6de-124">Accept</span></span>|<span data-ttu-id="9a6de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a6de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a6de-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a6de-126">Request body</span></span>
<span data-ttu-id="9a6de-127">В теле запроса добавьте представление объекта managedIOSStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a6de-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="9a6de-128">Ниже показаны свойства, которые необходимо указывать при создании объекта managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="9a6de-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="9a6de-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a6de-129">Property</span></span>|<span data-ttu-id="9a6de-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9a6de-130">Type</span></span>|<span data-ttu-id="9a6de-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9a6de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a6de-132">id</span><span class="sxs-lookup"><span data-stu-id="9a6de-132">id</span></span>|<span data-ttu-id="9a6de-133">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-133">String</span></span>|<span data-ttu-id="9a6de-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9a6de-134">Key of the entity.</span></span> <span data-ttu-id="9a6de-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9a6de-136">displayName</span></span>|<span data-ttu-id="9a6de-137">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-137">String</span></span>|<span data-ttu-id="9a6de-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9a6de-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9a6de-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-140">description</span><span class="sxs-lookup"><span data-stu-id="9a6de-140">description</span></span>|<span data-ttu-id="9a6de-141">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-141">String</span></span>|<span data-ttu-id="9a6de-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-142">The description of the app.</span></span> <span data-ttu-id="9a6de-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9a6de-144">publisher</span></span>|<span data-ttu-id="9a6de-145">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-145">String</span></span>|<span data-ttu-id="9a6de-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-146">The publisher of the app.</span></span> <span data-ttu-id="9a6de-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9a6de-148">largeIcon</span></span>|[<span data-ttu-id="9a6de-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9a6de-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9a6de-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9a6de-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9a6de-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a6de-152">createdDateTime</span></span>|<span data-ttu-id="9a6de-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a6de-153">DateTimeOffset</span></span>|<span data-ttu-id="9a6de-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-154">The date and time the app was created.</span></span> <span data-ttu-id="9a6de-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a6de-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9a6de-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a6de-157">DateTimeOffset</span></span>|<span data-ttu-id="9a6de-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9a6de-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9a6de-160">isFeatured</span></span>|<span data-ttu-id="9a6de-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a6de-161">Boolean</span></span>|<span data-ttu-id="9a6de-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9a6de-163">privacyInformationUrl</span></span>|<span data-ttu-id="9a6de-164">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-164">String</span></span>|<span data-ttu-id="9a6de-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9a6de-165">The privacy statement Url.</span></span> <span data-ttu-id="9a6de-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9a6de-167">informationUrl</span></span>|<span data-ttu-id="9a6de-168">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-168">String</span></span>|<span data-ttu-id="9a6de-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9a6de-169">The more information Url.</span></span> <span data-ttu-id="9a6de-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-171">owner</span><span class="sxs-lookup"><span data-stu-id="9a6de-171">owner</span></span>|<span data-ttu-id="9a6de-172">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-172">String</span></span>|<span data-ttu-id="9a6de-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-173">The owner of the app.</span></span> <span data-ttu-id="9a6de-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-175">developer</span><span class="sxs-lookup"><span data-stu-id="9a6de-175">developer</span></span>|<span data-ttu-id="9a6de-176">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-176">String</span></span>|<span data-ttu-id="9a6de-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-177">The developer of the app.</span></span> <span data-ttu-id="9a6de-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-179">notes</span><span class="sxs-lookup"><span data-stu-id="9a6de-179">notes</span></span>|<span data-ttu-id="9a6de-180">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-180">String</span></span>|<span data-ttu-id="9a6de-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-181">Notes for the app.</span></span> <span data-ttu-id="9a6de-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a6de-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="9a6de-183">publishingState</span></span>|[<span data-ttu-id="9a6de-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9a6de-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9a6de-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-185">The publishing state for the app.</span></span> <span data-ttu-id="9a6de-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9a6de-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9a6de-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9a6de-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9a6de-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9a6de-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9a6de-189">appAvailability</span></span>|[<span data-ttu-id="9a6de-190">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="9a6de-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9a6de-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-191">The Application's availability.</span></span> <span data-ttu-id="9a6de-192">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a6de-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9a6de-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9a6de-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9a6de-194">version</span><span class="sxs-lookup"><span data-stu-id="9a6de-194">version</span></span>|<span data-ttu-id="9a6de-195">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-195">String</span></span>|<span data-ttu-id="9a6de-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-196">The Application's version.</span></span> <span data-ttu-id="9a6de-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a6de-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9a6de-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="9a6de-198">bundleId</span></span>|<span data-ttu-id="9a6de-199">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-199">String</span></span>|<span data-ttu-id="9a6de-200">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="9a6de-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="9a6de-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9a6de-201">appStoreUrl</span></span>|<span data-ttu-id="9a6de-202">String</span><span class="sxs-lookup"><span data-stu-id="9a6de-202">String</span></span>|<span data-ttu-id="9a6de-203">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="9a6de-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="9a6de-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9a6de-204">applicableDeviceType</span></span>|[<span data-ttu-id="9a6de-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9a6de-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9a6de-206">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9a6de-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9a6de-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a6de-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9a6de-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a6de-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9a6de-209">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9a6de-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9a6de-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a6de-210">Response</span></span>
<span data-ttu-id="9a6de-211">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9a6de-211">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a6de-212">Пример</span><span class="sxs-lookup"><span data-stu-id="9a6de-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a6de-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a6de-213">Request</span></span>
<span data-ttu-id="9a6de-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a6de-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="9a6de-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a6de-215">Response</span></span>
<span data-ttu-id="9a6de-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a6de-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









