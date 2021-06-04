---
title: Update managedAndroidLobApp
description: Обновление свойств объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6eaaebdf0c40d5f99184ad87a0454e38fc9514b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754317"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="48299-103">Update managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="48299-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="48299-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48299-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48299-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48299-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48299-106">Обновление свойств объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48299-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48299-107">Prerequisites</span></span>
<span data-ttu-id="48299-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48299-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48299-110">Permission type</span></span>|<span data-ttu-id="48299-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48299-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48299-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48299-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48299-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48299-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48299-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48299-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48299-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48299-115">Not supported.</span></span>|
|<span data-ttu-id="48299-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="48299-116">Application</span></span>|<span data-ttu-id="48299-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48299-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48299-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48299-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="48299-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="48299-119">Request headers</span></span>
|<span data-ttu-id="48299-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48299-120">Header</span></span>|<span data-ttu-id="48299-121">Значение</span><span class="sxs-lookup"><span data-stu-id="48299-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48299-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48299-122">Authorization</span></span>|<span data-ttu-id="48299-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48299-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48299-124">Accept</span><span class="sxs-lookup"><span data-stu-id="48299-124">Accept</span></span>|<span data-ttu-id="48299-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48299-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48299-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48299-126">Request body</span></span>
<span data-ttu-id="48299-127">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48299-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="48299-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="48299-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="48299-129">Property</span></span>|<span data-ttu-id="48299-130">Тип</span><span class="sxs-lookup"><span data-stu-id="48299-130">Type</span></span>|<span data-ttu-id="48299-131">Описание</span><span class="sxs-lookup"><span data-stu-id="48299-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48299-132">id</span><span class="sxs-lookup"><span data-stu-id="48299-132">id</span></span>|<span data-ttu-id="48299-133">String</span><span class="sxs-lookup"><span data-stu-id="48299-133">String</span></span>|<span data-ttu-id="48299-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48299-134">Key of the entity.</span></span> <span data-ttu-id="48299-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-136">displayName</span><span class="sxs-lookup"><span data-stu-id="48299-136">displayName</span></span>|<span data-ttu-id="48299-137">String</span><span class="sxs-lookup"><span data-stu-id="48299-137">String</span></span>|<span data-ttu-id="48299-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="48299-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="48299-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-140">description</span><span class="sxs-lookup"><span data-stu-id="48299-140">description</span></span>|<span data-ttu-id="48299-141">String</span><span class="sxs-lookup"><span data-stu-id="48299-141">String</span></span>|<span data-ttu-id="48299-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-142">The description of the app.</span></span> <span data-ttu-id="48299-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-144">publisher</span><span class="sxs-lookup"><span data-stu-id="48299-144">publisher</span></span>|<span data-ttu-id="48299-145">String</span><span class="sxs-lookup"><span data-stu-id="48299-145">String</span></span>|<span data-ttu-id="48299-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-146">The publisher of the app.</span></span> <span data-ttu-id="48299-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48299-148">largeIcon</span></span>|[<span data-ttu-id="48299-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48299-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48299-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="48299-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="48299-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48299-152">createdDateTime</span></span>|<span data-ttu-id="48299-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48299-153">DateTimeOffset</span></span>|<span data-ttu-id="48299-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-154">The date and time the app was created.</span></span> <span data-ttu-id="48299-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48299-156">lastModifiedDateTime</span></span>|<span data-ttu-id="48299-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48299-157">DateTimeOffset</span></span>|<span data-ttu-id="48299-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-158">The date and time the app was last modified.</span></span> <span data-ttu-id="48299-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48299-160">isFeatured</span></span>|<span data-ttu-id="48299-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="48299-161">Boolean</span></span>|<span data-ttu-id="48299-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48299-163">privacyInformationUrl</span></span>|<span data-ttu-id="48299-164">String</span><span class="sxs-lookup"><span data-stu-id="48299-164">String</span></span>|<span data-ttu-id="48299-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="48299-165">The privacy statement Url.</span></span> <span data-ttu-id="48299-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48299-167">informationUrl</span></span>|<span data-ttu-id="48299-168">String</span><span class="sxs-lookup"><span data-stu-id="48299-168">String</span></span>|<span data-ttu-id="48299-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="48299-169">The more information Url.</span></span> <span data-ttu-id="48299-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-171">owner</span><span class="sxs-lookup"><span data-stu-id="48299-171">owner</span></span>|<span data-ttu-id="48299-172">String</span><span class="sxs-lookup"><span data-stu-id="48299-172">String</span></span>|<span data-ttu-id="48299-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-173">The owner of the app.</span></span> <span data-ttu-id="48299-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-175">developer</span><span class="sxs-lookup"><span data-stu-id="48299-175">developer</span></span>|<span data-ttu-id="48299-176">String</span><span class="sxs-lookup"><span data-stu-id="48299-176">String</span></span>|<span data-ttu-id="48299-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-177">The developer of the app.</span></span> <span data-ttu-id="48299-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-179">notes</span><span class="sxs-lookup"><span data-stu-id="48299-179">notes</span></span>|<span data-ttu-id="48299-180">String</span><span class="sxs-lookup"><span data-stu-id="48299-180">String</span></span>|<span data-ttu-id="48299-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-181">Notes for the app.</span></span> <span data-ttu-id="48299-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48299-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="48299-183">publishingState</span></span>|[<span data-ttu-id="48299-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48299-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48299-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-185">The publishing state for the app.</span></span> <span data-ttu-id="48299-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="48299-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48299-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="48299-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="48299-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48299-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="48299-189">appAvailability</span></span>|[<span data-ttu-id="48299-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="48299-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="48299-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-191">The Application's availability.</span></span> <span data-ttu-id="48299-192">Унаследованный от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="48299-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="48299-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="48299-194">version</span><span class="sxs-lookup"><span data-stu-id="48299-194">version</span></span>|<span data-ttu-id="48299-195">String</span><span class="sxs-lookup"><span data-stu-id="48299-195">String</span></span>|<span data-ttu-id="48299-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-196">The Application's version.</span></span> <span data-ttu-id="48299-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="48299-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="48299-198">committedContentVersion</span></span>|<span data-ttu-id="48299-199">String</span><span class="sxs-lookup"><span data-stu-id="48299-199">String</span></span>|<span data-ttu-id="48299-200">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="48299-200">The internal committed content version.</span></span> <span data-ttu-id="48299-201">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="48299-202">fileName</span><span class="sxs-lookup"><span data-stu-id="48299-202">fileName</span></span>|<span data-ttu-id="48299-203">String</span><span class="sxs-lookup"><span data-stu-id="48299-203">String</span></span>|<span data-ttu-id="48299-204">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="48299-204">The name of the main Lob application file.</span></span> <span data-ttu-id="48299-205">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="48299-206">size</span><span class="sxs-lookup"><span data-stu-id="48299-206">size</span></span>|<span data-ttu-id="48299-207">Int64</span><span class="sxs-lookup"><span data-stu-id="48299-207">Int64</span></span>|<span data-ttu-id="48299-208">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="48299-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="48299-209">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48299-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="48299-210">packageId</span><span class="sxs-lookup"><span data-stu-id="48299-210">packageId</span></span>|<span data-ttu-id="48299-211">String</span><span class="sxs-lookup"><span data-stu-id="48299-211">String</span></span>|<span data-ttu-id="48299-212">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="48299-212">The package identifier.</span></span>|
|<span data-ttu-id="48299-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="48299-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="48299-214">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="48299-214">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="48299-215">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="48299-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="48299-216">versionName</span><span class="sxs-lookup"><span data-stu-id="48299-216">versionName</span></span>|<span data-ttu-id="48299-217">String</span><span class="sxs-lookup"><span data-stu-id="48299-217">String</span></span>|<span data-ttu-id="48299-218">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="48299-218">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="48299-219">versionCode</span><span class="sxs-lookup"><span data-stu-id="48299-219">versionCode</span></span>|<span data-ttu-id="48299-220">String</span><span class="sxs-lookup"><span data-stu-id="48299-220">String</span></span>|<span data-ttu-id="48299-221">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="48299-221">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="48299-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="48299-222">Response</span></span>
<span data-ttu-id="48299-223">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48299-223">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48299-224">Пример</span><span class="sxs-lookup"><span data-stu-id="48299-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="48299-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="48299-225">Request</span></span>
<span data-ttu-id="48299-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48299-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1193

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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="48299-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="48299-227">Response</span></span>
<span data-ttu-id="48299-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48299-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1365

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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




