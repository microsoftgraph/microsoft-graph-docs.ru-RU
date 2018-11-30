---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
ms.openlocfilehash: 0822bbc0679f1cb19ec8e4c3d217a3bf5661cdaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027852"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="e0623-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e0623-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="e0623-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e0623-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0623-105">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0623-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e0623-106">Prerequisites</span></span>
<span data-ttu-id="e0623-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0623-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0623-109">Permission type</span></span>|<span data-ttu-id="e0623-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0623-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0623-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0623-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0623-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0623-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0623-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0623-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0623-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0623-114">Not supported.</span></span>|
|<span data-ttu-id="e0623-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0623-115">Application</span></span>|<span data-ttu-id="e0623-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0623-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0623-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0623-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e0623-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0623-118">Request headers</span></span>
|<span data-ttu-id="e0623-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0623-119">Header</span></span>|<span data-ttu-id="e0623-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e0623-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0623-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0623-121">Authorization</span></span>|<span data-ttu-id="e0623-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e0623-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0623-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e0623-123">Accept</span></span>|<span data-ttu-id="e0623-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e0623-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0623-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0623-125">Request body</span></span>
<span data-ttu-id="e0623-126">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0623-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="e0623-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="e0623-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="e0623-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0623-128">Property</span></span>|<span data-ttu-id="e0623-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e0623-129">Type</span></span>|<span data-ttu-id="e0623-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e0623-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0623-131">id</span><span class="sxs-lookup"><span data-stu-id="e0623-131">id</span></span>|<span data-ttu-id="e0623-132">String</span><span class="sxs-lookup"><span data-stu-id="e0623-132">String</span></span>|<span data-ttu-id="e0623-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0623-133">Key of the entity.</span></span> <span data-ttu-id="e0623-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e0623-135">displayName</span></span>|<span data-ttu-id="e0623-136">String</span><span class="sxs-lookup"><span data-stu-id="e0623-136">String</span></span>|<span data-ttu-id="e0623-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e0623-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e0623-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-139">описание</span><span class="sxs-lookup"><span data-stu-id="e0623-139">description</span></span>|<span data-ttu-id="e0623-140">String</span><span class="sxs-lookup"><span data-stu-id="e0623-140">String</span></span>|<span data-ttu-id="e0623-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-141">The description of the app.</span></span> <span data-ttu-id="e0623-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e0623-143">publisher</span></span>|<span data-ttu-id="e0623-144">String</span><span class="sxs-lookup"><span data-stu-id="e0623-144">String</span></span>|<span data-ttu-id="e0623-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-145">The publisher of the app.</span></span> <span data-ttu-id="e0623-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e0623-147">largeIcon</span></span>|[<span data-ttu-id="e0623-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e0623-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e0623-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e0623-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e0623-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0623-151">createdDateTime</span></span>|<span data-ttu-id="e0623-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0623-152">DateTimeOffset</span></span>|<span data-ttu-id="e0623-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-153">The date and time the app was created.</span></span> <span data-ttu-id="e0623-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0623-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e0623-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0623-156">DateTimeOffset</span></span>|<span data-ttu-id="e0623-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e0623-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e0623-159">isFeatured</span></span>|<span data-ttu-id="e0623-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0623-160">Boolean</span></span>|<span data-ttu-id="e0623-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e0623-162">privacyInformationUrl</span></span>|<span data-ttu-id="e0623-163">String</span><span class="sxs-lookup"><span data-stu-id="e0623-163">String</span></span>|<span data-ttu-id="e0623-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e0623-164">The privacy statement Url.</span></span> <span data-ttu-id="e0623-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e0623-166">informationUrl</span></span>|<span data-ttu-id="e0623-167">String</span><span class="sxs-lookup"><span data-stu-id="e0623-167">String</span></span>|<span data-ttu-id="e0623-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e0623-168">The more information Url.</span></span> <span data-ttu-id="e0623-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-170">owner</span><span class="sxs-lookup"><span data-stu-id="e0623-170">owner</span></span>|<span data-ttu-id="e0623-171">String</span><span class="sxs-lookup"><span data-stu-id="e0623-171">String</span></span>|<span data-ttu-id="e0623-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-172">The owner of the app.</span></span> <span data-ttu-id="e0623-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-174">developer</span><span class="sxs-lookup"><span data-stu-id="e0623-174">developer</span></span>|<span data-ttu-id="e0623-175">String</span><span class="sxs-lookup"><span data-stu-id="e0623-175">String</span></span>|<span data-ttu-id="e0623-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-176">The developer of the app.</span></span> <span data-ttu-id="e0623-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-178">notes</span><span class="sxs-lookup"><span data-stu-id="e0623-178">notes</span></span>|<span data-ttu-id="e0623-179">String</span><span class="sxs-lookup"><span data-stu-id="e0623-179">String</span></span>|<span data-ttu-id="e0623-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e0623-180">Notes for the app.</span></span> <span data-ttu-id="e0623-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e0623-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e0623-182">publishingState</span></span>|[<span data-ttu-id="e0623-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e0623-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e0623-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-184">The publishing state for the app.</span></span> <span data-ttu-id="e0623-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e0623-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e0623-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e0623-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e0623-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e0623-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e0623-188">appAvailability</span></span>|[<span data-ttu-id="e0623-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e0623-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e0623-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-190">The Application's availability.</span></span> <span data-ttu-id="e0623-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e0623-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e0623-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e0623-193">version</span><span class="sxs-lookup"><span data-stu-id="e0623-193">version</span></span>|<span data-ttu-id="e0623-194">String</span><span class="sxs-lookup"><span data-stu-id="e0623-194">String</span></span>|<span data-ttu-id="e0623-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-195">The Application's version.</span></span> <span data-ttu-id="e0623-196">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e0623-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e0623-197">committedContentVersion</span></span>|<span data-ttu-id="e0623-198">String</span><span class="sxs-lookup"><span data-stu-id="e0623-198">String</span></span>|<span data-ttu-id="e0623-199">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e0623-199">The internal committed content version.</span></span> <span data-ttu-id="e0623-200">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e0623-201">fileName</span><span class="sxs-lookup"><span data-stu-id="e0623-201">fileName</span></span>|<span data-ttu-id="e0623-202">String</span><span class="sxs-lookup"><span data-stu-id="e0623-202">String</span></span>|<span data-ttu-id="e0623-203">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e0623-203">The name of the main Lob application file.</span></span> <span data-ttu-id="e0623-204">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e0623-205">size</span><span class="sxs-lookup"><span data-stu-id="e0623-205">size</span></span>|<span data-ttu-id="e0623-206">Int64</span><span class="sxs-lookup"><span data-stu-id="e0623-206">Int64</span></span>|<span data-ttu-id="e0623-207">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e0623-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="e0623-208">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0623-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e0623-209">packageId</span><span class="sxs-lookup"><span data-stu-id="e0623-209">packageId</span></span>|<span data-ttu-id="e0623-210">String</span><span class="sxs-lookup"><span data-stu-id="e0623-210">String</span></span>|<span data-ttu-id="e0623-211">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="e0623-211">The package identifier.</span></span>|
|<span data-ttu-id="e0623-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e0623-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e0623-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e0623-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e0623-214">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e0623-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e0623-215">versionName</span><span class="sxs-lookup"><span data-stu-id="e0623-215">versionName</span></span>|<span data-ttu-id="e0623-216">String</span><span class="sxs-lookup"><span data-stu-id="e0623-216">String</span></span>|<span data-ttu-id="e0623-217">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="e0623-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e0623-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="e0623-218">versionCode</span></span>|<span data-ttu-id="e0623-219">String</span><span class="sxs-lookup"><span data-stu-id="e0623-219">String</span></span>|<span data-ttu-id="e0623-220">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="e0623-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e0623-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0623-221">Response</span></span>
<span data-ttu-id="e0623-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e0623-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0623-223">Пример</span><span class="sxs-lookup"><span data-stu-id="e0623-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0623-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0623-224">Request</span></span>
<span data-ttu-id="e0623-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0623-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="e0623-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0623-226">Response</span></span>
<span data-ttu-id="e0623-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e0623-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



