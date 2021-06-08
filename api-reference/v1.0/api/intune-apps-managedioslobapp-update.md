---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1eb39ba619dd00cd5759d5e4aeb12ba3645ec5b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759800"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="58774-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="58774-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="58774-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58774-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58774-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58774-106">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58774-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="58774-107">Prerequisites</span></span>
<span data-ttu-id="58774-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58774-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58774-110">Permission type</span></span>|<span data-ttu-id="58774-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58774-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58774-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58774-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58774-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58774-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58774-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58774-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58774-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58774-115">Not supported.</span></span>|
|<span data-ttu-id="58774-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="58774-116">Application</span></span>|<span data-ttu-id="58774-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58774-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58774-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58774-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="58774-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58774-119">Request headers</span></span>
|<span data-ttu-id="58774-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58774-120">Header</span></span>|<span data-ttu-id="58774-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58774-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58774-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58774-122">Authorization</span></span>|<span data-ttu-id="58774-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58774-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58774-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58774-124">Accept</span></span>|<span data-ttu-id="58774-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58774-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58774-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58774-126">Request body</span></span>
<span data-ttu-id="58774-127">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58774-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="58774-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="58774-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58774-129">Property</span></span>|<span data-ttu-id="58774-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58774-130">Type</span></span>|<span data-ttu-id="58774-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58774-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58774-132">id</span><span class="sxs-lookup"><span data-stu-id="58774-132">id</span></span>|<span data-ttu-id="58774-133">String</span><span class="sxs-lookup"><span data-stu-id="58774-133">String</span></span>|<span data-ttu-id="58774-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58774-134">Key of the entity.</span></span> <span data-ttu-id="58774-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-136">displayName</span><span class="sxs-lookup"><span data-stu-id="58774-136">displayName</span></span>|<span data-ttu-id="58774-137">String</span><span class="sxs-lookup"><span data-stu-id="58774-137">String</span></span>|<span data-ttu-id="58774-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="58774-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="58774-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-140">description</span><span class="sxs-lookup"><span data-stu-id="58774-140">description</span></span>|<span data-ttu-id="58774-141">String</span><span class="sxs-lookup"><span data-stu-id="58774-141">String</span></span>|<span data-ttu-id="58774-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-142">The description of the app.</span></span> <span data-ttu-id="58774-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-144">publisher</span><span class="sxs-lookup"><span data-stu-id="58774-144">publisher</span></span>|<span data-ttu-id="58774-145">String</span><span class="sxs-lookup"><span data-stu-id="58774-145">String</span></span>|<span data-ttu-id="58774-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-146">The publisher of the app.</span></span> <span data-ttu-id="58774-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="58774-148">largeIcon</span></span>|[<span data-ttu-id="58774-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="58774-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="58774-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="58774-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="58774-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58774-152">createdDateTime</span></span>|<span data-ttu-id="58774-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58774-153">DateTimeOffset</span></span>|<span data-ttu-id="58774-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-154">The date and time the app was created.</span></span> <span data-ttu-id="58774-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58774-156">lastModifiedDateTime</span></span>|<span data-ttu-id="58774-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58774-157">DateTimeOffset</span></span>|<span data-ttu-id="58774-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-158">The date and time the app was last modified.</span></span> <span data-ttu-id="58774-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="58774-160">isFeatured</span></span>|<span data-ttu-id="58774-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="58774-161">Boolean</span></span>|<span data-ttu-id="58774-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="58774-163">privacyInformationUrl</span></span>|<span data-ttu-id="58774-164">String</span><span class="sxs-lookup"><span data-stu-id="58774-164">String</span></span>|<span data-ttu-id="58774-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="58774-165">The privacy statement Url.</span></span> <span data-ttu-id="58774-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="58774-167">informationUrl</span></span>|<span data-ttu-id="58774-168">String</span><span class="sxs-lookup"><span data-stu-id="58774-168">String</span></span>|<span data-ttu-id="58774-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="58774-169">The more information Url.</span></span> <span data-ttu-id="58774-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-171">owner</span><span class="sxs-lookup"><span data-stu-id="58774-171">owner</span></span>|<span data-ttu-id="58774-172">String</span><span class="sxs-lookup"><span data-stu-id="58774-172">String</span></span>|<span data-ttu-id="58774-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-173">The owner of the app.</span></span> <span data-ttu-id="58774-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-175">developer</span><span class="sxs-lookup"><span data-stu-id="58774-175">developer</span></span>|<span data-ttu-id="58774-176">String</span><span class="sxs-lookup"><span data-stu-id="58774-176">String</span></span>|<span data-ttu-id="58774-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-177">The developer of the app.</span></span> <span data-ttu-id="58774-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-179">notes</span><span class="sxs-lookup"><span data-stu-id="58774-179">notes</span></span>|<span data-ttu-id="58774-180">String</span><span class="sxs-lookup"><span data-stu-id="58774-180">String</span></span>|<span data-ttu-id="58774-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-181">Notes for the app.</span></span> <span data-ttu-id="58774-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58774-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="58774-183">publishingState</span></span>|[<span data-ttu-id="58774-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="58774-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="58774-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-185">The publishing state for the app.</span></span> <span data-ttu-id="58774-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="58774-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="58774-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="58774-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="58774-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="58774-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="58774-189">appAvailability</span></span>|[<span data-ttu-id="58774-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="58774-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="58774-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-191">The Application's availability.</span></span> <span data-ttu-id="58774-192">Унаследованный от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="58774-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="58774-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="58774-194">version</span><span class="sxs-lookup"><span data-stu-id="58774-194">version</span></span>|<span data-ttu-id="58774-195">String</span><span class="sxs-lookup"><span data-stu-id="58774-195">String</span></span>|<span data-ttu-id="58774-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-196">The Application's version.</span></span> <span data-ttu-id="58774-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="58774-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="58774-198">committedContentVersion</span></span>|<span data-ttu-id="58774-199">String</span><span class="sxs-lookup"><span data-stu-id="58774-199">String</span></span>|<span data-ttu-id="58774-200">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="58774-200">The internal committed content version.</span></span> <span data-ttu-id="58774-201">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58774-202">fileName</span><span class="sxs-lookup"><span data-stu-id="58774-202">fileName</span></span>|<span data-ttu-id="58774-203">String</span><span class="sxs-lookup"><span data-stu-id="58774-203">String</span></span>|<span data-ttu-id="58774-204">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="58774-204">The name of the main Lob application file.</span></span> <span data-ttu-id="58774-205">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58774-206">size</span><span class="sxs-lookup"><span data-stu-id="58774-206">size</span></span>|<span data-ttu-id="58774-207">Int64</span><span class="sxs-lookup"><span data-stu-id="58774-207">Int64</span></span>|<span data-ttu-id="58774-208">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="58774-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="58774-209">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58774-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58774-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="58774-210">bundleId</span></span>|<span data-ttu-id="58774-211">String</span><span class="sxs-lookup"><span data-stu-id="58774-211">String</span></span>|<span data-ttu-id="58774-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="58774-212">The Identity Name.</span></span>|
|<span data-ttu-id="58774-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="58774-213">applicableDeviceType</span></span>|[<span data-ttu-id="58774-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="58774-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="58774-215">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="58774-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="58774-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58774-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="58774-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58774-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="58774-218">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="58774-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="58774-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58774-219">expirationDateTime</span></span>|<span data-ttu-id="58774-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58774-220">DateTimeOffset</span></span>|<span data-ttu-id="58774-221">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="58774-221">The expiration time.</span></span>|
|<span data-ttu-id="58774-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="58774-222">versionNumber</span></span>|<span data-ttu-id="58774-223">String</span><span class="sxs-lookup"><span data-stu-id="58774-223">String</span></span>|<span data-ttu-id="58774-224">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="58774-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="58774-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="58774-225">buildNumber</span></span>|<span data-ttu-id="58774-226">String</span><span class="sxs-lookup"><span data-stu-id="58774-226">String</span></span>|<span data-ttu-id="58774-227">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="58774-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="58774-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="58774-228">Response</span></span>
<span data-ttu-id="58774-229">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="58774-229">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58774-230">Пример</span><span class="sxs-lookup"><span data-stu-id="58774-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="58774-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="58774-231">Request</span></span>
<span data-ttu-id="58774-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58774-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1327

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
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="58774-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="58774-233">Response</span></span>
<span data-ttu-id="58774-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58774-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1499

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
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```




