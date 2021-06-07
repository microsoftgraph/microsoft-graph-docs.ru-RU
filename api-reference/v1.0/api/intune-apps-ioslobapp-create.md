---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83244489322e33db138672c7630b09c018264f54
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757425"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="e5f75-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="e5f75-103">Create iosLobApp</span></span>

<span data-ttu-id="e5f75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5f75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5f75-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5f75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5f75-106">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5f75-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5f75-107">Prerequisites</span></span>
<span data-ttu-id="e5f75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5f75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5f75-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5f75-110">Permission type</span></span>|<span data-ttu-id="e5f75-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5f75-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5f75-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5f75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5f75-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5f75-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5f75-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5f75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5f75-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5f75-115">Not supported.</span></span>|
|<span data-ttu-id="e5f75-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5f75-116">Application</span></span>|<span data-ttu-id="e5f75-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5f75-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5f75-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5f75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e5f75-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5f75-119">Request headers</span></span>
|<span data-ttu-id="e5f75-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5f75-120">Header</span></span>|<span data-ttu-id="e5f75-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5f75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5f75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5f75-122">Authorization</span></span>|<span data-ttu-id="e5f75-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5f75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5f75-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5f75-124">Accept</span></span>|<span data-ttu-id="e5f75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5f75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5f75-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5f75-126">Request body</span></span>
<span data-ttu-id="e5f75-127">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5f75-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="e5f75-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="e5f75-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="e5f75-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5f75-129">Property</span></span>|<span data-ttu-id="e5f75-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5f75-130">Type</span></span>|<span data-ttu-id="e5f75-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5f75-132">id</span><span class="sxs-lookup"><span data-stu-id="e5f75-132">id</span></span>|<span data-ttu-id="e5f75-133">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-133">String</span></span>|<span data-ttu-id="e5f75-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5f75-134">Key of the entity.</span></span> <span data-ttu-id="e5f75-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e5f75-136">displayName</span></span>|<span data-ttu-id="e5f75-137">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-137">String</span></span>|<span data-ttu-id="e5f75-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e5f75-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e5f75-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-140">description</span><span class="sxs-lookup"><span data-stu-id="e5f75-140">description</span></span>|<span data-ttu-id="e5f75-141">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-141">String</span></span>|<span data-ttu-id="e5f75-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-142">The description of the app.</span></span> <span data-ttu-id="e5f75-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e5f75-144">publisher</span></span>|<span data-ttu-id="e5f75-145">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-145">String</span></span>|<span data-ttu-id="e5f75-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-146">The publisher of the app.</span></span> <span data-ttu-id="e5f75-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e5f75-148">largeIcon</span></span>|[<span data-ttu-id="e5f75-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e5f75-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e5f75-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e5f75-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e5f75-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f75-152">createdDateTime</span></span>|<span data-ttu-id="e5f75-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f75-153">DateTimeOffset</span></span>|<span data-ttu-id="e5f75-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-154">The date and time the app was created.</span></span> <span data-ttu-id="e5f75-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f75-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e5f75-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f75-157">DateTimeOffset</span></span>|<span data-ttu-id="e5f75-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e5f75-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e5f75-160">isFeatured</span></span>|<span data-ttu-id="e5f75-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5f75-161">Boolean</span></span>|<span data-ttu-id="e5f75-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e5f75-163">privacyInformationUrl</span></span>|<span data-ttu-id="e5f75-164">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-164">String</span></span>|<span data-ttu-id="e5f75-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e5f75-165">The privacy statement Url.</span></span> <span data-ttu-id="e5f75-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e5f75-167">informationUrl</span></span>|<span data-ttu-id="e5f75-168">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-168">String</span></span>|<span data-ttu-id="e5f75-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e5f75-169">The more information Url.</span></span> <span data-ttu-id="e5f75-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-171">owner</span><span class="sxs-lookup"><span data-stu-id="e5f75-171">owner</span></span>|<span data-ttu-id="e5f75-172">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-172">String</span></span>|<span data-ttu-id="e5f75-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-173">The owner of the app.</span></span> <span data-ttu-id="e5f75-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-175">developer</span><span class="sxs-lookup"><span data-stu-id="e5f75-175">developer</span></span>|<span data-ttu-id="e5f75-176">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-176">String</span></span>|<span data-ttu-id="e5f75-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-177">The developer of the app.</span></span> <span data-ttu-id="e5f75-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-179">notes</span><span class="sxs-lookup"><span data-stu-id="e5f75-179">notes</span></span>|<span data-ttu-id="e5f75-180">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-180">String</span></span>|<span data-ttu-id="e5f75-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-181">Notes for the app.</span></span> <span data-ttu-id="e5f75-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5f75-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="e5f75-183">publishingState</span></span>|[<span data-ttu-id="e5f75-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e5f75-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e5f75-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-185">The publishing state for the app.</span></span> <span data-ttu-id="e5f75-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e5f75-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e5f75-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e5f75-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e5f75-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e5f75-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e5f75-189">committedContentVersion</span></span>|<span data-ttu-id="e5f75-190">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-190">String</span></span>|<span data-ttu-id="e5f75-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e5f75-191">The internal committed content version.</span></span> <span data-ttu-id="e5f75-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5f75-193">fileName</span><span class="sxs-lookup"><span data-stu-id="e5f75-193">fileName</span></span>|<span data-ttu-id="e5f75-194">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-194">String</span></span>|<span data-ttu-id="e5f75-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-195">The name of the main Lob application file.</span></span> <span data-ttu-id="e5f75-196">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5f75-197">size</span><span class="sxs-lookup"><span data-stu-id="e5f75-197">size</span></span>|<span data-ttu-id="e5f75-198">Int64</span><span class="sxs-lookup"><span data-stu-id="e5f75-198">Int64</span></span>|<span data-ttu-id="e5f75-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e5f75-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="e5f75-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5f75-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5f75-201">bundleId</span><span class="sxs-lookup"><span data-stu-id="e5f75-201">bundleId</span></span>|<span data-ttu-id="e5f75-202">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-202">String</span></span>|<span data-ttu-id="e5f75-203">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e5f75-203">The Identity Name.</span></span>|
|<span data-ttu-id="e5f75-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e5f75-204">applicableDeviceType</span></span>|[<span data-ttu-id="e5f75-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e5f75-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e5f75-206">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e5f75-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="e5f75-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e5f75-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e5f75-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e5f75-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="e5f75-209">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e5f75-209">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e5f75-210">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e5f75-210">expirationDateTime</span></span>|<span data-ttu-id="e5f75-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5f75-211">DateTimeOffset</span></span>|<span data-ttu-id="e5f75-212">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="e5f75-212">The expiration time.</span></span>|
|<span data-ttu-id="e5f75-213">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e5f75-213">versionNumber</span></span>|<span data-ttu-id="e5f75-214">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-214">String</span></span>|<span data-ttu-id="e5f75-215">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="e5f75-215">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e5f75-216">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e5f75-216">buildNumber</span></span>|<span data-ttu-id="e5f75-217">String</span><span class="sxs-lookup"><span data-stu-id="e5f75-217">String</span></span>|<span data-ttu-id="e5f75-218">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="e5f75-218">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e5f75-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5f75-219">Response</span></span>
<span data-ttu-id="e5f75-220">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5f75-220">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5f75-221">Пример</span><span class="sxs-lookup"><span data-stu-id="e5f75-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5f75-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5f75-222">Request</span></span>
<span data-ttu-id="e5f75-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5f75-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1249

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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

### <a name="response"></a><span data-ttu-id="e5f75-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5f75-224">Response</span></span>
<span data-ttu-id="e5f75-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5f75-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1421

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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




