---
title: Create managedIOSLobApp
description: Создание объекта managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c113c8c76029ee7a0d1c5f3e5d0b1d0ab5f31bba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987078"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="79d67-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="79d67-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="79d67-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79d67-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79d67-105">Создание объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-105">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79d67-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="79d67-106">Prerequisites</span></span>
<span data-ttu-id="79d67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79d67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79d67-109">Permission type</span></span>|<span data-ttu-id="79d67-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79d67-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79d67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79d67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79d67-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79d67-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79d67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79d67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79d67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d67-114">Not supported.</span></span>|
|<span data-ttu-id="79d67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79d67-115">Application</span></span>|<span data-ttu-id="79d67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79d67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79d67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79d67-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="79d67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79d67-118">Request headers</span></span>
|<span data-ttu-id="79d67-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79d67-119">Header</span></span>|<span data-ttu-id="79d67-120">Значение</span><span class="sxs-lookup"><span data-stu-id="79d67-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79d67-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79d67-121">Authorization</span></span>|<span data-ttu-id="79d67-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="79d67-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79d67-123">Accept</span><span class="sxs-lookup"><span data-stu-id="79d67-123">Accept</span></span>|<span data-ttu-id="79d67-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79d67-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79d67-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79d67-125">Request body</span></span>
<span data-ttu-id="79d67-126">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79d67-126">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="79d67-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="79d67-127">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="79d67-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="79d67-128">Property</span></span>|<span data-ttu-id="79d67-129">Тип</span><span class="sxs-lookup"><span data-stu-id="79d67-129">Type</span></span>|<span data-ttu-id="79d67-130">Описание</span><span class="sxs-lookup"><span data-stu-id="79d67-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79d67-131">id</span><span class="sxs-lookup"><span data-stu-id="79d67-131">id</span></span>|<span data-ttu-id="79d67-132">Строка</span><span class="sxs-lookup"><span data-stu-id="79d67-132">String</span></span>|<span data-ttu-id="79d67-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79d67-133">Key of the entity.</span></span> <span data-ttu-id="79d67-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-135">displayName</span><span class="sxs-lookup"><span data-stu-id="79d67-135">displayName</span></span>|<span data-ttu-id="79d67-136">String</span><span class="sxs-lookup"><span data-stu-id="79d67-136">String</span></span>|<span data-ttu-id="79d67-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="79d67-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="79d67-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-139">описание</span><span class="sxs-lookup"><span data-stu-id="79d67-139">description</span></span>|<span data-ttu-id="79d67-140">String</span><span class="sxs-lookup"><span data-stu-id="79d67-140">String</span></span>|<span data-ttu-id="79d67-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-141">The description of the app.</span></span> <span data-ttu-id="79d67-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-143">publisher</span><span class="sxs-lookup"><span data-stu-id="79d67-143">publisher</span></span>|<span data-ttu-id="79d67-144">String</span><span class="sxs-lookup"><span data-stu-id="79d67-144">String</span></span>|<span data-ttu-id="79d67-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-145">The publisher of the app.</span></span> <span data-ttu-id="79d67-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="79d67-147">largeIcon</span></span>|[<span data-ttu-id="79d67-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="79d67-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="79d67-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="79d67-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="79d67-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79d67-151">createdDateTime</span></span>|<span data-ttu-id="79d67-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d67-152">DateTimeOffset</span></span>|<span data-ttu-id="79d67-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-153">The date and time the app was created.</span></span> <span data-ttu-id="79d67-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79d67-155">lastModifiedDateTime</span></span>|<span data-ttu-id="79d67-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d67-156">DateTimeOffset</span></span>|<span data-ttu-id="79d67-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-157">The date and time the app was last modified.</span></span> <span data-ttu-id="79d67-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="79d67-159">isFeatured</span></span>|<span data-ttu-id="79d67-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d67-160">Boolean</span></span>|<span data-ttu-id="79d67-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="79d67-162">privacyInformationUrl</span></span>|<span data-ttu-id="79d67-163">String</span><span class="sxs-lookup"><span data-stu-id="79d67-163">String</span></span>|<span data-ttu-id="79d67-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="79d67-164">The privacy statement Url.</span></span> <span data-ttu-id="79d67-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="79d67-166">informationUrl</span></span>|<span data-ttu-id="79d67-167">String</span><span class="sxs-lookup"><span data-stu-id="79d67-167">String</span></span>|<span data-ttu-id="79d67-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="79d67-168">The more information Url.</span></span> <span data-ttu-id="79d67-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-170">owner</span><span class="sxs-lookup"><span data-stu-id="79d67-170">owner</span></span>|<span data-ttu-id="79d67-171">String</span><span class="sxs-lookup"><span data-stu-id="79d67-171">String</span></span>|<span data-ttu-id="79d67-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-172">The owner of the app.</span></span> <span data-ttu-id="79d67-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-174">developer</span><span class="sxs-lookup"><span data-stu-id="79d67-174">developer</span></span>|<span data-ttu-id="79d67-175">String</span><span class="sxs-lookup"><span data-stu-id="79d67-175">String</span></span>|<span data-ttu-id="79d67-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-176">The developer of the app.</span></span> <span data-ttu-id="79d67-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-178">notes</span><span class="sxs-lookup"><span data-stu-id="79d67-178">notes</span></span>|<span data-ttu-id="79d67-179">String</span><span class="sxs-lookup"><span data-stu-id="79d67-179">String</span></span>|<span data-ttu-id="79d67-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="79d67-180">Notes for the app.</span></span> <span data-ttu-id="79d67-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79d67-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="79d67-182">publishingState</span></span>|[<span data-ttu-id="79d67-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="79d67-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="79d67-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-184">The publishing state for the app.</span></span> <span data-ttu-id="79d67-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="79d67-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="79d67-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="79d67-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="79d67-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="79d67-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="79d67-188">appAvailability</span></span>|[<span data-ttu-id="79d67-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="79d67-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="79d67-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-190">The Application's availability.</span></span> <span data-ttu-id="79d67-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="79d67-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="79d67-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="79d67-193">version</span><span class="sxs-lookup"><span data-stu-id="79d67-193">version</span></span>|<span data-ttu-id="79d67-194">String</span><span class="sxs-lookup"><span data-stu-id="79d67-194">String</span></span>|<span data-ttu-id="79d67-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-195">The Application's version.</span></span> <span data-ttu-id="79d67-196">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="79d67-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="79d67-197">committedContentVersion</span></span>|<span data-ttu-id="79d67-198">String</span><span class="sxs-lookup"><span data-stu-id="79d67-198">String</span></span>|<span data-ttu-id="79d67-199">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="79d67-199">The internal committed content version.</span></span> <span data-ttu-id="79d67-200">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="79d67-201">fileName</span><span class="sxs-lookup"><span data-stu-id="79d67-201">fileName</span></span>|<span data-ttu-id="79d67-202">String</span><span class="sxs-lookup"><span data-stu-id="79d67-202">String</span></span>|<span data-ttu-id="79d67-203">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="79d67-203">The name of the main Lob application file.</span></span> <span data-ttu-id="79d67-204">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="79d67-205">size</span><span class="sxs-lookup"><span data-stu-id="79d67-205">size</span></span>|<span data-ttu-id="79d67-206">Int64</span><span class="sxs-lookup"><span data-stu-id="79d67-206">Int64</span></span>|<span data-ttu-id="79d67-207">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="79d67-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="79d67-208">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="79d67-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="79d67-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="79d67-209">bundleId</span></span>|<span data-ttu-id="79d67-210">String</span><span class="sxs-lookup"><span data-stu-id="79d67-210">String</span></span>|<span data-ttu-id="79d67-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="79d67-211">The Identity Name.</span></span>|
|<span data-ttu-id="79d67-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="79d67-212">applicableDeviceType</span></span>|[<span data-ttu-id="79d67-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="79d67-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="79d67-214">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="79d67-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="79d67-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79d67-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="79d67-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79d67-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="79d67-217">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="79d67-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="79d67-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="79d67-218">expirationDateTime</span></span>|<span data-ttu-id="79d67-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d67-219">DateTimeOffset</span></span>|<span data-ttu-id="79d67-220">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="79d67-220">The expiration time.</span></span>|
|<span data-ttu-id="79d67-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="79d67-221">versionNumber</span></span>|<span data-ttu-id="79d67-222">String</span><span class="sxs-lookup"><span data-stu-id="79d67-222">String</span></span>|<span data-ttu-id="79d67-223">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="79d67-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="79d67-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="79d67-224">buildNumber</span></span>|<span data-ttu-id="79d67-225">String</span><span class="sxs-lookup"><span data-stu-id="79d67-225">String</span></span>|<span data-ttu-id="79d67-226">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="79d67-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="79d67-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="79d67-227">Response</span></span>
<span data-ttu-id="79d67-228">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="79d67-228">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79d67-229">Пример</span><span class="sxs-lookup"><span data-stu-id="79d67-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="79d67-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="79d67-230">Request</span></span>
<span data-ttu-id="79d67-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79d67-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1287

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="79d67-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="79d67-232">Response</span></span>
<span data-ttu-id="79d67-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79d67-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



