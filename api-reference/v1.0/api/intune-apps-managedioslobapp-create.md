---
title: Create managedIOSLobApp
description: Создание объекта managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa411d23440d68d25ee43ec767ae2c68053f74c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260496"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="bb536-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="bb536-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="bb536-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb536-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb536-105">Создание объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-105">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb536-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bb536-106">Prerequisites</span></span>
<span data-ttu-id="bb536-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb536-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb536-109">Permission type</span></span>|<span data-ttu-id="bb536-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb536-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb536-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb536-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb536-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb536-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb536-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb536-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb536-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb536-114">Not supported.</span></span>|
|<span data-ttu-id="bb536-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb536-115">Application</span></span>|<span data-ttu-id="bb536-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb536-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb536-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb536-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bb536-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb536-118">Request headers</span></span>
|<span data-ttu-id="bb536-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb536-119">Header</span></span>|<span data-ttu-id="bb536-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bb536-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb536-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb536-121">Authorization</span></span>|<span data-ttu-id="bb536-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bb536-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb536-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb536-123">Accept</span></span>|<span data-ttu-id="bb536-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb536-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb536-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb536-125">Request body</span></span>
<span data-ttu-id="bb536-126">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb536-126">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="bb536-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="bb536-127">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="bb536-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb536-128">Property</span></span>|<span data-ttu-id="bb536-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bb536-129">Type</span></span>|<span data-ttu-id="bb536-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bb536-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb536-131">id</span><span class="sxs-lookup"><span data-stu-id="bb536-131">id</span></span>|<span data-ttu-id="bb536-132">Строка</span><span class="sxs-lookup"><span data-stu-id="bb536-132">String</span></span>|<span data-ttu-id="bb536-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb536-133">Key of the entity.</span></span> <span data-ttu-id="bb536-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bb536-135">displayName</span></span>|<span data-ttu-id="bb536-136">String</span><span class="sxs-lookup"><span data-stu-id="bb536-136">String</span></span>|<span data-ttu-id="bb536-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="bb536-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bb536-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-139">description</span><span class="sxs-lookup"><span data-stu-id="bb536-139">description</span></span>|<span data-ttu-id="bb536-140">Строка</span><span class="sxs-lookup"><span data-stu-id="bb536-140">String</span></span>|<span data-ttu-id="bb536-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-141">The description of the app.</span></span> <span data-ttu-id="bb536-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-143">publisher</span><span class="sxs-lookup"><span data-stu-id="bb536-143">publisher</span></span>|<span data-ttu-id="bb536-144">String</span><span class="sxs-lookup"><span data-stu-id="bb536-144">String</span></span>|<span data-ttu-id="bb536-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-145">The publisher of the app.</span></span> <span data-ttu-id="bb536-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bb536-147">largeIcon</span></span>|[<span data-ttu-id="bb536-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bb536-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bb536-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="bb536-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bb536-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb536-151">createdDateTime</span></span>|<span data-ttu-id="bb536-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb536-152">DateTimeOffset</span></span>|<span data-ttu-id="bb536-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-153">The date and time the app was created.</span></span> <span data-ttu-id="bb536-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb536-155">lastModifiedDateTime</span></span>|<span data-ttu-id="bb536-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb536-156">DateTimeOffset</span></span>|<span data-ttu-id="bb536-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-157">The date and time the app was last modified.</span></span> <span data-ttu-id="bb536-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bb536-159">isFeatured</span></span>|<span data-ttu-id="bb536-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb536-160">Boolean</span></span>|<span data-ttu-id="bb536-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bb536-162">privacyInformationUrl</span></span>|<span data-ttu-id="bb536-163">String</span><span class="sxs-lookup"><span data-stu-id="bb536-163">String</span></span>|<span data-ttu-id="bb536-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="bb536-164">The privacy statement Url.</span></span> <span data-ttu-id="bb536-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bb536-166">informationUrl</span></span>|<span data-ttu-id="bb536-167">String</span><span class="sxs-lookup"><span data-stu-id="bb536-167">String</span></span>|<span data-ttu-id="bb536-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="bb536-168">The more information Url.</span></span> <span data-ttu-id="bb536-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-170">owner</span><span class="sxs-lookup"><span data-stu-id="bb536-170">owner</span></span>|<span data-ttu-id="bb536-171">String</span><span class="sxs-lookup"><span data-stu-id="bb536-171">String</span></span>|<span data-ttu-id="bb536-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-172">The owner of the app.</span></span> <span data-ttu-id="bb536-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-174">developer</span><span class="sxs-lookup"><span data-stu-id="bb536-174">developer</span></span>|<span data-ttu-id="bb536-175">String</span><span class="sxs-lookup"><span data-stu-id="bb536-175">String</span></span>|<span data-ttu-id="bb536-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-176">The developer of the app.</span></span> <span data-ttu-id="bb536-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-178">notes</span><span class="sxs-lookup"><span data-stu-id="bb536-178">notes</span></span>|<span data-ttu-id="bb536-179">String</span><span class="sxs-lookup"><span data-stu-id="bb536-179">String</span></span>|<span data-ttu-id="bb536-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="bb536-180">Notes for the app.</span></span> <span data-ttu-id="bb536-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb536-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="bb536-182">publishingState</span></span>|[<span data-ttu-id="bb536-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="bb536-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bb536-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-184">The publishing state for the app.</span></span> <span data-ttu-id="bb536-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="bb536-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bb536-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bb536-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bb536-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bb536-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bb536-188">appAvailability</span></span>|[<span data-ttu-id="bb536-189">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="bb536-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="bb536-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-190">The Application's availability.</span></span> <span data-ttu-id="bb536-191">НаСледуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="bb536-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bb536-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bb536-193">version</span><span class="sxs-lookup"><span data-stu-id="bb536-193">version</span></span>|<span data-ttu-id="bb536-194">Строка</span><span class="sxs-lookup"><span data-stu-id="bb536-194">String</span></span>|<span data-ttu-id="bb536-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-195">The Application's version.</span></span> <span data-ttu-id="bb536-196">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="bb536-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bb536-197">committedContentVersion</span></span>|<span data-ttu-id="bb536-198">String</span><span class="sxs-lookup"><span data-stu-id="bb536-198">String</span></span>|<span data-ttu-id="bb536-199">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="bb536-199">The internal committed content version.</span></span> <span data-ttu-id="bb536-200">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bb536-201">fileName</span><span class="sxs-lookup"><span data-stu-id="bb536-201">fileName</span></span>|<span data-ttu-id="bb536-202">String</span><span class="sxs-lookup"><span data-stu-id="bb536-202">String</span></span>|<span data-ttu-id="bb536-203">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="bb536-203">The name of the main Lob application file.</span></span> <span data-ttu-id="bb536-204">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bb536-205">size</span><span class="sxs-lookup"><span data-stu-id="bb536-205">size</span></span>|<span data-ttu-id="bb536-206">Int64</span><span class="sxs-lookup"><span data-stu-id="bb536-206">Int64</span></span>|<span data-ttu-id="bb536-207">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="bb536-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="bb536-208">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb536-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bb536-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="bb536-209">bundleId</span></span>|<span data-ttu-id="bb536-210">String</span><span class="sxs-lookup"><span data-stu-id="bb536-210">String</span></span>|<span data-ttu-id="bb536-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bb536-211">The Identity Name.</span></span>|
|<span data-ttu-id="bb536-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="bb536-212">applicableDeviceType</span></span>|[<span data-ttu-id="bb536-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="bb536-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="bb536-214">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="bb536-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="bb536-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb536-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bb536-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb536-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="bb536-217">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="bb536-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bb536-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb536-218">expirationDateTime</span></span>|<span data-ttu-id="bb536-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb536-219">DateTimeOffset</span></span>|<span data-ttu-id="bb536-220">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="bb536-220">The expiration time.</span></span>|
|<span data-ttu-id="bb536-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="bb536-221">versionNumber</span></span>|<span data-ttu-id="bb536-222">String</span><span class="sxs-lookup"><span data-stu-id="bb536-222">String</span></span>|<span data-ttu-id="bb536-223">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="bb536-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bb536-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="bb536-224">buildNumber</span></span>|<span data-ttu-id="bb536-225">String</span><span class="sxs-lookup"><span data-stu-id="bb536-225">String</span></span>|<span data-ttu-id="bb536-226">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="bb536-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="bb536-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb536-227">Response</span></span>
<span data-ttu-id="bb536-228">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bb536-228">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb536-229">Пример</span><span class="sxs-lookup"><span data-stu-id="bb536-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb536-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb536-230">Request</span></span>
<span data-ttu-id="bb536-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb536-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb536-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb536-232">Response</span></span>
<span data-ttu-id="bb536-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb536-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



