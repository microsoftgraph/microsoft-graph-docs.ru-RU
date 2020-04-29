---
title: Create managedIOSLobApp
description: Создание объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 63966fd441149f55fe635c0fbff2c2480719cd3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442644"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="07128-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="07128-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="07128-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07128-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07128-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07128-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07128-106">Создание объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07128-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="07128-107">Prerequisites</span></span>
<span data-ttu-id="07128-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07128-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07128-110">Permission type</span></span>|<span data-ttu-id="07128-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07128-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07128-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07128-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07128-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07128-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07128-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07128-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07128-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07128-115">Not supported.</span></span>|
|<span data-ttu-id="07128-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07128-116">Application</span></span>|<span data-ttu-id="07128-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07128-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07128-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07128-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="07128-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07128-119">Request headers</span></span>
|<span data-ttu-id="07128-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07128-120">Header</span></span>|<span data-ttu-id="07128-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07128-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07128-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07128-122">Authorization</span></span>|<span data-ttu-id="07128-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07128-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07128-124">Accept</span><span class="sxs-lookup"><span data-stu-id="07128-124">Accept</span></span>|<span data-ttu-id="07128-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07128-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07128-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07128-126">Request body</span></span>
<span data-ttu-id="07128-127">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07128-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="07128-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="07128-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="07128-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="07128-129">Property</span></span>|<span data-ttu-id="07128-130">Тип</span><span class="sxs-lookup"><span data-stu-id="07128-130">Type</span></span>|<span data-ttu-id="07128-131">Описание</span><span class="sxs-lookup"><span data-stu-id="07128-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07128-132">id</span><span class="sxs-lookup"><span data-stu-id="07128-132">id</span></span>|<span data-ttu-id="07128-133">Строка</span><span class="sxs-lookup"><span data-stu-id="07128-133">String</span></span>|<span data-ttu-id="07128-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="07128-134">Key of the entity.</span></span> <span data-ttu-id="07128-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-136">displayName</span><span class="sxs-lookup"><span data-stu-id="07128-136">displayName</span></span>|<span data-ttu-id="07128-137">Строка</span><span class="sxs-lookup"><span data-stu-id="07128-137">String</span></span>|<span data-ttu-id="07128-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="07128-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="07128-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-140">description</span><span class="sxs-lookup"><span data-stu-id="07128-140">description</span></span>|<span data-ttu-id="07128-141">String</span><span class="sxs-lookup"><span data-stu-id="07128-141">String</span></span>|<span data-ttu-id="07128-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-142">The description of the app.</span></span> <span data-ttu-id="07128-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-144">publisher</span><span class="sxs-lookup"><span data-stu-id="07128-144">publisher</span></span>|<span data-ttu-id="07128-145">String</span><span class="sxs-lookup"><span data-stu-id="07128-145">String</span></span>|<span data-ttu-id="07128-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-146">The publisher of the app.</span></span> <span data-ttu-id="07128-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="07128-148">largeIcon</span></span>|[<span data-ttu-id="07128-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07128-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07128-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="07128-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="07128-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07128-152">createdDateTime</span></span>|<span data-ttu-id="07128-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07128-153">DateTimeOffset</span></span>|<span data-ttu-id="07128-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-154">The date and time the app was created.</span></span> <span data-ttu-id="07128-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07128-156">lastModifiedDateTime</span></span>|<span data-ttu-id="07128-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07128-157">DateTimeOffset</span></span>|<span data-ttu-id="07128-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-158">The date and time the app was last modified.</span></span> <span data-ttu-id="07128-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="07128-160">isFeatured</span></span>|<span data-ttu-id="07128-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="07128-161">Boolean</span></span>|<span data-ttu-id="07128-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="07128-163">privacyInformationUrl</span></span>|<span data-ttu-id="07128-164">String</span><span class="sxs-lookup"><span data-stu-id="07128-164">String</span></span>|<span data-ttu-id="07128-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="07128-165">The privacy statement Url.</span></span> <span data-ttu-id="07128-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="07128-167">informationUrl</span></span>|<span data-ttu-id="07128-168">String</span><span class="sxs-lookup"><span data-stu-id="07128-168">String</span></span>|<span data-ttu-id="07128-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="07128-169">The more information Url.</span></span> <span data-ttu-id="07128-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-171">owner</span><span class="sxs-lookup"><span data-stu-id="07128-171">owner</span></span>|<span data-ttu-id="07128-172">String</span><span class="sxs-lookup"><span data-stu-id="07128-172">String</span></span>|<span data-ttu-id="07128-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-173">The owner of the app.</span></span> <span data-ttu-id="07128-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-175">developer</span><span class="sxs-lookup"><span data-stu-id="07128-175">developer</span></span>|<span data-ttu-id="07128-176">String</span><span class="sxs-lookup"><span data-stu-id="07128-176">String</span></span>|<span data-ttu-id="07128-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-177">The developer of the app.</span></span> <span data-ttu-id="07128-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-179">notes</span><span class="sxs-lookup"><span data-stu-id="07128-179">notes</span></span>|<span data-ttu-id="07128-180">String</span><span class="sxs-lookup"><span data-stu-id="07128-180">String</span></span>|<span data-ttu-id="07128-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-181">Notes for the app.</span></span> <span data-ttu-id="07128-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="07128-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="07128-183">publishingState</span></span>|[<span data-ttu-id="07128-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="07128-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="07128-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-185">The publishing state for the app.</span></span> <span data-ttu-id="07128-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="07128-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="07128-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="07128-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="07128-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="07128-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="07128-189">appAvailability</span></span>|[<span data-ttu-id="07128-190">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="07128-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="07128-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-191">The Application's availability.</span></span> <span data-ttu-id="07128-192">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="07128-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="07128-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="07128-194">version</span><span class="sxs-lookup"><span data-stu-id="07128-194">version</span></span>|<span data-ttu-id="07128-195">String</span><span class="sxs-lookup"><span data-stu-id="07128-195">String</span></span>|<span data-ttu-id="07128-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-196">The Application's version.</span></span> <span data-ttu-id="07128-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="07128-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="07128-198">committedContentVersion</span></span>|<span data-ttu-id="07128-199">String</span><span class="sxs-lookup"><span data-stu-id="07128-199">String</span></span>|<span data-ttu-id="07128-200">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="07128-200">The internal committed content version.</span></span> <span data-ttu-id="07128-201">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="07128-202">fileName</span><span class="sxs-lookup"><span data-stu-id="07128-202">fileName</span></span>|<span data-ttu-id="07128-203">String</span><span class="sxs-lookup"><span data-stu-id="07128-203">String</span></span>|<span data-ttu-id="07128-204">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="07128-204">The name of the main Lob application file.</span></span> <span data-ttu-id="07128-205">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="07128-206">size</span><span class="sxs-lookup"><span data-stu-id="07128-206">size</span></span>|<span data-ttu-id="07128-207">Int64</span><span class="sxs-lookup"><span data-stu-id="07128-207">Int64</span></span>|<span data-ttu-id="07128-208">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="07128-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="07128-209">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="07128-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="07128-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="07128-210">bundleId</span></span>|<span data-ttu-id="07128-211">String</span><span class="sxs-lookup"><span data-stu-id="07128-211">String</span></span>|<span data-ttu-id="07128-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="07128-212">The Identity Name.</span></span>|
|<span data-ttu-id="07128-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="07128-213">applicableDeviceType</span></span>|[<span data-ttu-id="07128-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="07128-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="07128-215">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="07128-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="07128-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="07128-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="07128-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="07128-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="07128-218">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="07128-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="07128-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="07128-219">expirationDateTime</span></span>|<span data-ttu-id="07128-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07128-220">DateTimeOffset</span></span>|<span data-ttu-id="07128-221">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="07128-221">The expiration time.</span></span>|
|<span data-ttu-id="07128-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="07128-222">versionNumber</span></span>|<span data-ttu-id="07128-223">String</span><span class="sxs-lookup"><span data-stu-id="07128-223">String</span></span>|<span data-ttu-id="07128-224">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="07128-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="07128-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="07128-225">buildNumber</span></span>|<span data-ttu-id="07128-226">String</span><span class="sxs-lookup"><span data-stu-id="07128-226">String</span></span>|<span data-ttu-id="07128-227">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="07128-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="07128-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="07128-228">Response</span></span>
<span data-ttu-id="07128-229">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="07128-229">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07128-230">Пример</span><span class="sxs-lookup"><span data-stu-id="07128-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="07128-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="07128-231">Request</span></span>
<span data-ttu-id="07128-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07128-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07128-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="07128-233">Response</span></span>
<span data-ttu-id="07128-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07128-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






