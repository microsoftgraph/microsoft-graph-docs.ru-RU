---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09f43dfce5dd9d7572882e668c4a28b40c485d2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442568"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="50401-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="50401-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="50401-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50401-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50401-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50401-106">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50401-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="50401-107">Prerequisites</span></span>
<span data-ttu-id="50401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50401-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50401-110">Permission type</span></span>|<span data-ttu-id="50401-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50401-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50401-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50401-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50401-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50401-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50401-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50401-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50401-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50401-115">Not supported.</span></span>|
|<span data-ttu-id="50401-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50401-116">Application</span></span>|<span data-ttu-id="50401-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50401-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50401-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50401-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="50401-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50401-119">Request headers</span></span>
|<span data-ttu-id="50401-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50401-120">Header</span></span>|<span data-ttu-id="50401-121">Значение</span><span class="sxs-lookup"><span data-stu-id="50401-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50401-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50401-122">Authorization</span></span>|<span data-ttu-id="50401-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50401-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50401-124">Accept</span><span class="sxs-lookup"><span data-stu-id="50401-124">Accept</span></span>|<span data-ttu-id="50401-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50401-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50401-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50401-126">Request body</span></span>
<span data-ttu-id="50401-127">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50401-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="50401-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="50401-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="50401-129">Property</span></span>|<span data-ttu-id="50401-130">Тип</span><span class="sxs-lookup"><span data-stu-id="50401-130">Type</span></span>|<span data-ttu-id="50401-131">Описание</span><span class="sxs-lookup"><span data-stu-id="50401-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50401-132">id</span><span class="sxs-lookup"><span data-stu-id="50401-132">id</span></span>|<span data-ttu-id="50401-133">Строка</span><span class="sxs-lookup"><span data-stu-id="50401-133">String</span></span>|<span data-ttu-id="50401-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50401-134">Key of the entity.</span></span> <span data-ttu-id="50401-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-136">displayName</span><span class="sxs-lookup"><span data-stu-id="50401-136">displayName</span></span>|<span data-ttu-id="50401-137">Строка</span><span class="sxs-lookup"><span data-stu-id="50401-137">String</span></span>|<span data-ttu-id="50401-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="50401-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="50401-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-140">description</span><span class="sxs-lookup"><span data-stu-id="50401-140">description</span></span>|<span data-ttu-id="50401-141">String</span><span class="sxs-lookup"><span data-stu-id="50401-141">String</span></span>|<span data-ttu-id="50401-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-142">The description of the app.</span></span> <span data-ttu-id="50401-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-144">publisher</span><span class="sxs-lookup"><span data-stu-id="50401-144">publisher</span></span>|<span data-ttu-id="50401-145">String</span><span class="sxs-lookup"><span data-stu-id="50401-145">String</span></span>|<span data-ttu-id="50401-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-146">The publisher of the app.</span></span> <span data-ttu-id="50401-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="50401-148">largeIcon</span></span>|[<span data-ttu-id="50401-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="50401-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="50401-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="50401-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="50401-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50401-152">createdDateTime</span></span>|<span data-ttu-id="50401-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50401-153">DateTimeOffset</span></span>|<span data-ttu-id="50401-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-154">The date and time the app was created.</span></span> <span data-ttu-id="50401-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50401-156">lastModifiedDateTime</span></span>|<span data-ttu-id="50401-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50401-157">DateTimeOffset</span></span>|<span data-ttu-id="50401-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-158">The date and time the app was last modified.</span></span> <span data-ttu-id="50401-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="50401-160">isFeatured</span></span>|<span data-ttu-id="50401-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="50401-161">Boolean</span></span>|<span data-ttu-id="50401-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="50401-163">privacyInformationUrl</span></span>|<span data-ttu-id="50401-164">String</span><span class="sxs-lookup"><span data-stu-id="50401-164">String</span></span>|<span data-ttu-id="50401-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="50401-165">The privacy statement Url.</span></span> <span data-ttu-id="50401-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="50401-167">informationUrl</span></span>|<span data-ttu-id="50401-168">String</span><span class="sxs-lookup"><span data-stu-id="50401-168">String</span></span>|<span data-ttu-id="50401-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="50401-169">The more information Url.</span></span> <span data-ttu-id="50401-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-171">owner</span><span class="sxs-lookup"><span data-stu-id="50401-171">owner</span></span>|<span data-ttu-id="50401-172">String</span><span class="sxs-lookup"><span data-stu-id="50401-172">String</span></span>|<span data-ttu-id="50401-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-173">The owner of the app.</span></span> <span data-ttu-id="50401-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-175">developer</span><span class="sxs-lookup"><span data-stu-id="50401-175">developer</span></span>|<span data-ttu-id="50401-176">String</span><span class="sxs-lookup"><span data-stu-id="50401-176">String</span></span>|<span data-ttu-id="50401-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-177">The developer of the app.</span></span> <span data-ttu-id="50401-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-179">notes</span><span class="sxs-lookup"><span data-stu-id="50401-179">notes</span></span>|<span data-ttu-id="50401-180">String</span><span class="sxs-lookup"><span data-stu-id="50401-180">String</span></span>|<span data-ttu-id="50401-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-181">Notes for the app.</span></span> <span data-ttu-id="50401-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="50401-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="50401-183">publishingState</span></span>|[<span data-ttu-id="50401-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="50401-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="50401-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-185">The publishing state for the app.</span></span> <span data-ttu-id="50401-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="50401-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="50401-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="50401-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="50401-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="50401-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="50401-189">appAvailability</span></span>|[<span data-ttu-id="50401-190">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="50401-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="50401-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-191">The Application's availability.</span></span> <span data-ttu-id="50401-192">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="50401-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="50401-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="50401-194">version</span><span class="sxs-lookup"><span data-stu-id="50401-194">version</span></span>|<span data-ttu-id="50401-195">String</span><span class="sxs-lookup"><span data-stu-id="50401-195">String</span></span>|<span data-ttu-id="50401-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-196">The Application's version.</span></span> <span data-ttu-id="50401-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="50401-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="50401-198">committedContentVersion</span></span>|<span data-ttu-id="50401-199">String</span><span class="sxs-lookup"><span data-stu-id="50401-199">String</span></span>|<span data-ttu-id="50401-200">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="50401-200">The internal committed content version.</span></span> <span data-ttu-id="50401-201">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="50401-202">fileName</span><span class="sxs-lookup"><span data-stu-id="50401-202">fileName</span></span>|<span data-ttu-id="50401-203">String</span><span class="sxs-lookup"><span data-stu-id="50401-203">String</span></span>|<span data-ttu-id="50401-204">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="50401-204">The name of the main Lob application file.</span></span> <span data-ttu-id="50401-205">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="50401-206">size</span><span class="sxs-lookup"><span data-stu-id="50401-206">size</span></span>|<span data-ttu-id="50401-207">Int64</span><span class="sxs-lookup"><span data-stu-id="50401-207">Int64</span></span>|<span data-ttu-id="50401-208">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="50401-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="50401-209">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="50401-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="50401-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="50401-210">bundleId</span></span>|<span data-ttu-id="50401-211">String</span><span class="sxs-lookup"><span data-stu-id="50401-211">String</span></span>|<span data-ttu-id="50401-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="50401-212">The Identity Name.</span></span>|
|<span data-ttu-id="50401-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="50401-213">applicableDeviceType</span></span>|[<span data-ttu-id="50401-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="50401-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="50401-215">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="50401-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="50401-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50401-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="50401-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50401-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="50401-218">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="50401-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="50401-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="50401-219">expirationDateTime</span></span>|<span data-ttu-id="50401-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50401-220">DateTimeOffset</span></span>|<span data-ttu-id="50401-221">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="50401-221">The expiration time.</span></span>|
|<span data-ttu-id="50401-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="50401-222">versionNumber</span></span>|<span data-ttu-id="50401-223">String</span><span class="sxs-lookup"><span data-stu-id="50401-223">String</span></span>|<span data-ttu-id="50401-224">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="50401-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="50401-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="50401-225">buildNumber</span></span>|<span data-ttu-id="50401-226">String</span><span class="sxs-lookup"><span data-stu-id="50401-226">String</span></span>|<span data-ttu-id="50401-227">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="50401-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="50401-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="50401-228">Response</span></span>
<span data-ttu-id="50401-229">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50401-229">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50401-230">Пример</span><span class="sxs-lookup"><span data-stu-id="50401-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="50401-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="50401-231">Request</span></span>
<span data-ttu-id="50401-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50401-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1307

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="50401-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="50401-233">Response</span></span>
<span data-ttu-id="50401-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50401-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1479

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```






