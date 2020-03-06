---
title: Create managedIOSLobApp
description: Создание объекта managedIOSLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95fa9e71d51d264f86803ae85070eea2f515798f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516203"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="957bd-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="957bd-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="957bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="957bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="957bd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="957bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="957bd-106">Создание объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="957bd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="957bd-107">Prerequisites</span></span>
<span data-ttu-id="957bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="957bd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="957bd-110">Permission type</span></span>|<span data-ttu-id="957bd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="957bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="957bd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="957bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="957bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="957bd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="957bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="957bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="957bd-115">Not supported.</span></span>|
|<span data-ttu-id="957bd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="957bd-116">Application</span></span>|<span data-ttu-id="957bd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="957bd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="957bd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="957bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="957bd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="957bd-119">Request headers</span></span>
|<span data-ttu-id="957bd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="957bd-120">Header</span></span>|<span data-ttu-id="957bd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="957bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="957bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="957bd-122">Authorization</span></span>|<span data-ttu-id="957bd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="957bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="957bd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="957bd-124">Accept</span></span>|<span data-ttu-id="957bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="957bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="957bd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="957bd-126">Request body</span></span>
<span data-ttu-id="957bd-127">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="957bd-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="957bd-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="957bd-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="957bd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="957bd-129">Property</span></span>|<span data-ttu-id="957bd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="957bd-130">Type</span></span>|<span data-ttu-id="957bd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="957bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="957bd-132">id</span><span class="sxs-lookup"><span data-stu-id="957bd-132">id</span></span>|<span data-ttu-id="957bd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-133">String</span></span>|<span data-ttu-id="957bd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="957bd-134">Key of the entity.</span></span> <span data-ttu-id="957bd-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="957bd-136">displayName</span></span>|<span data-ttu-id="957bd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-137">String</span></span>|<span data-ttu-id="957bd-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="957bd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="957bd-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-140">description</span><span class="sxs-lookup"><span data-stu-id="957bd-140">description</span></span>|<span data-ttu-id="957bd-141">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-141">String</span></span>|<span data-ttu-id="957bd-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-142">The description of the app.</span></span> <span data-ttu-id="957bd-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="957bd-144">publisher</span></span>|<span data-ttu-id="957bd-145">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-145">String</span></span>|<span data-ttu-id="957bd-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-146">The publisher of the app.</span></span> <span data-ttu-id="957bd-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="957bd-148">largeIcon</span></span>|[<span data-ttu-id="957bd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="957bd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="957bd-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="957bd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="957bd-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="957bd-152">createdDateTime</span></span>|<span data-ttu-id="957bd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="957bd-153">DateTimeOffset</span></span>|<span data-ttu-id="957bd-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-154">The date and time the app was created.</span></span> <span data-ttu-id="957bd-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="957bd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="957bd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="957bd-157">DateTimeOffset</span></span>|<span data-ttu-id="957bd-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="957bd-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="957bd-160">isFeatured</span></span>|<span data-ttu-id="957bd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="957bd-161">Boolean</span></span>|<span data-ttu-id="957bd-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="957bd-163">privacyInformationUrl</span></span>|<span data-ttu-id="957bd-164">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-164">String</span></span>|<span data-ttu-id="957bd-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="957bd-165">The privacy statement Url.</span></span> <span data-ttu-id="957bd-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="957bd-167">informationUrl</span></span>|<span data-ttu-id="957bd-168">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-168">String</span></span>|<span data-ttu-id="957bd-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="957bd-169">The more information Url.</span></span> <span data-ttu-id="957bd-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-171">owner</span><span class="sxs-lookup"><span data-stu-id="957bd-171">owner</span></span>|<span data-ttu-id="957bd-172">String</span><span class="sxs-lookup"><span data-stu-id="957bd-172">String</span></span>|<span data-ttu-id="957bd-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-173">The owner of the app.</span></span> <span data-ttu-id="957bd-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-175">developer</span><span class="sxs-lookup"><span data-stu-id="957bd-175">developer</span></span>|<span data-ttu-id="957bd-176">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-176">String</span></span>|<span data-ttu-id="957bd-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-177">The developer of the app.</span></span> <span data-ttu-id="957bd-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-179">notes</span><span class="sxs-lookup"><span data-stu-id="957bd-179">notes</span></span>|<span data-ttu-id="957bd-180">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-180">String</span></span>|<span data-ttu-id="957bd-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-181">Notes for the app.</span></span> <span data-ttu-id="957bd-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="957bd-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="957bd-183">publishingState</span></span>|[<span data-ttu-id="957bd-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="957bd-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="957bd-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-185">The publishing state for the app.</span></span> <span data-ttu-id="957bd-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="957bd-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="957bd-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="957bd-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="957bd-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="957bd-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="957bd-189">appAvailability</span></span>|[<span data-ttu-id="957bd-190">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="957bd-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="957bd-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-191">The Application's availability.</span></span> <span data-ttu-id="957bd-192">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="957bd-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="957bd-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="957bd-194">version</span><span class="sxs-lookup"><span data-stu-id="957bd-194">version</span></span>|<span data-ttu-id="957bd-195">String</span><span class="sxs-lookup"><span data-stu-id="957bd-195">String</span></span>|<span data-ttu-id="957bd-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-196">The Application's version.</span></span> <span data-ttu-id="957bd-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="957bd-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="957bd-198">committedContentVersion</span></span>|<span data-ttu-id="957bd-199">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-199">String</span></span>|<span data-ttu-id="957bd-200">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="957bd-200">The internal committed content version.</span></span> <span data-ttu-id="957bd-201">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="957bd-202">fileName</span><span class="sxs-lookup"><span data-stu-id="957bd-202">fileName</span></span>|<span data-ttu-id="957bd-203">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-203">String</span></span>|<span data-ttu-id="957bd-204">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="957bd-204">The name of the main Lob application file.</span></span> <span data-ttu-id="957bd-205">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="957bd-206">size</span><span class="sxs-lookup"><span data-stu-id="957bd-206">size</span></span>|<span data-ttu-id="957bd-207">Int64</span><span class="sxs-lookup"><span data-stu-id="957bd-207">Int64</span></span>|<span data-ttu-id="957bd-208">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="957bd-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="957bd-209">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="957bd-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="957bd-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="957bd-210">bundleId</span></span>|<span data-ttu-id="957bd-211">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-211">String</span></span>|<span data-ttu-id="957bd-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="957bd-212">The Identity Name.</span></span>|
|<span data-ttu-id="957bd-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="957bd-213">applicableDeviceType</span></span>|[<span data-ttu-id="957bd-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="957bd-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="957bd-215">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="957bd-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="957bd-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="957bd-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="957bd-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="957bd-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="957bd-218">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="957bd-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="957bd-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="957bd-219">expirationDateTime</span></span>|<span data-ttu-id="957bd-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="957bd-220">DateTimeOffset</span></span>|<span data-ttu-id="957bd-221">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="957bd-221">The expiration time.</span></span>|
|<span data-ttu-id="957bd-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="957bd-222">versionNumber</span></span>|<span data-ttu-id="957bd-223">Строка</span><span class="sxs-lookup"><span data-stu-id="957bd-223">String</span></span>|<span data-ttu-id="957bd-224">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="957bd-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="957bd-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="957bd-225">buildNumber</span></span>|<span data-ttu-id="957bd-226">String</span><span class="sxs-lookup"><span data-stu-id="957bd-226">String</span></span>|<span data-ttu-id="957bd-227">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="957bd-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="957bd-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="957bd-228">Response</span></span>
<span data-ttu-id="957bd-229">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="957bd-229">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="957bd-230">Пример</span><span class="sxs-lookup"><span data-stu-id="957bd-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="957bd-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="957bd-231">Request</span></span>
<span data-ttu-id="957bd-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="957bd-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="957bd-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="957bd-233">Response</span></span>
<span data-ttu-id="957bd-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="957bd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




