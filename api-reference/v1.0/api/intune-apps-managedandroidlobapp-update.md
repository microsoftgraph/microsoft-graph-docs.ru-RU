---
title: Update managedAndroidLobApp
description: Обновление свойств объекта managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b00e4bbe0b4dff1a45e9ffe89c59edc4379b1b89
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578612"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="9d114-103">Update managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="9d114-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="9d114-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d114-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d114-105">Обновление свойств объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d114-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9d114-106">Prerequisites</span></span>
<span data-ttu-id="9d114-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d114-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d114-109">Permission type</span></span>|<span data-ttu-id="9d114-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d114-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d114-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d114-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d114-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d114-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d114-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d114-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d114-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d114-114">Not supported.</span></span>|
|<span data-ttu-id="9d114-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d114-115">Application</span></span>|<span data-ttu-id="9d114-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d114-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d114-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d114-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9d114-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d114-118">Request headers</span></span>
|<span data-ttu-id="9d114-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d114-119">Header</span></span>|<span data-ttu-id="9d114-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9d114-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d114-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d114-121">Authorization</span></span>|<span data-ttu-id="9d114-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d114-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d114-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9d114-123">Accept</span></span>|<span data-ttu-id="9d114-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d114-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d114-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d114-125">Request body</span></span>
<span data-ttu-id="9d114-126">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d114-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="9d114-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="9d114-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d114-128">Property</span></span>|<span data-ttu-id="9d114-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9d114-129">Type</span></span>|<span data-ttu-id="9d114-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9d114-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d114-131">id</span><span class="sxs-lookup"><span data-stu-id="9d114-131">id</span></span>|<span data-ttu-id="9d114-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9d114-132">String</span></span>|<span data-ttu-id="9d114-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d114-133">Key of the entity.</span></span> <span data-ttu-id="9d114-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9d114-135">displayName</span></span>|<span data-ttu-id="9d114-136">String</span><span class="sxs-lookup"><span data-stu-id="9d114-136">String</span></span>|<span data-ttu-id="9d114-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9d114-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9d114-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-139">description</span><span class="sxs-lookup"><span data-stu-id="9d114-139">description</span></span>|<span data-ttu-id="9d114-140">String</span><span class="sxs-lookup"><span data-stu-id="9d114-140">String</span></span>|<span data-ttu-id="9d114-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-141">The description of the app.</span></span> <span data-ttu-id="9d114-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-143">publisher</span><span class="sxs-lookup"><span data-stu-id="9d114-143">publisher</span></span>|<span data-ttu-id="9d114-144">String</span><span class="sxs-lookup"><span data-stu-id="9d114-144">String</span></span>|<span data-ttu-id="9d114-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-145">The publisher of the app.</span></span> <span data-ttu-id="9d114-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9d114-147">largeIcon</span></span>|[<span data-ttu-id="9d114-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9d114-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9d114-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9d114-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9d114-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d114-151">createdDateTime</span></span>|<span data-ttu-id="9d114-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d114-152">DateTimeOffset</span></span>|<span data-ttu-id="9d114-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-153">The date and time the app was created.</span></span> <span data-ttu-id="9d114-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d114-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9d114-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d114-156">DateTimeOffset</span></span>|<span data-ttu-id="9d114-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-157">The date and time the app was last modified.</span></span> <span data-ttu-id="9d114-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9d114-159">isFeatured</span></span>|<span data-ttu-id="9d114-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d114-160">Boolean</span></span>|<span data-ttu-id="9d114-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9d114-162">privacyInformationUrl</span></span>|<span data-ttu-id="9d114-163">String</span><span class="sxs-lookup"><span data-stu-id="9d114-163">String</span></span>|<span data-ttu-id="9d114-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9d114-164">The privacy statement Url.</span></span> <span data-ttu-id="9d114-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9d114-166">informationUrl</span></span>|<span data-ttu-id="9d114-167">String</span><span class="sxs-lookup"><span data-stu-id="9d114-167">String</span></span>|<span data-ttu-id="9d114-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9d114-168">The more information Url.</span></span> <span data-ttu-id="9d114-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-170">owner</span><span class="sxs-lookup"><span data-stu-id="9d114-170">owner</span></span>|<span data-ttu-id="9d114-171">String</span><span class="sxs-lookup"><span data-stu-id="9d114-171">String</span></span>|<span data-ttu-id="9d114-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-172">The owner of the app.</span></span> <span data-ttu-id="9d114-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-174">developer</span><span class="sxs-lookup"><span data-stu-id="9d114-174">developer</span></span>|<span data-ttu-id="9d114-175">String</span><span class="sxs-lookup"><span data-stu-id="9d114-175">String</span></span>|<span data-ttu-id="9d114-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-176">The developer of the app.</span></span> <span data-ttu-id="9d114-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-178">notes</span><span class="sxs-lookup"><span data-stu-id="9d114-178">notes</span></span>|<span data-ttu-id="9d114-179">String</span><span class="sxs-lookup"><span data-stu-id="9d114-179">String</span></span>|<span data-ttu-id="9d114-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-180">Notes for the app.</span></span> <span data-ttu-id="9d114-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d114-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="9d114-182">publishingState</span></span>|[<span data-ttu-id="9d114-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9d114-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9d114-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-184">The publishing state for the app.</span></span> <span data-ttu-id="9d114-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9d114-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9d114-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9d114-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9d114-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9d114-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9d114-188">appAvailability</span></span>|[<span data-ttu-id="9d114-189">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="9d114-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9d114-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-190">The Application's availability.</span></span> <span data-ttu-id="9d114-191">НаСледуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9d114-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9d114-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9d114-193">version</span><span class="sxs-lookup"><span data-stu-id="9d114-193">version</span></span>|<span data-ttu-id="9d114-194">String</span><span class="sxs-lookup"><span data-stu-id="9d114-194">String</span></span>|<span data-ttu-id="9d114-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-195">The Application's version.</span></span> <span data-ttu-id="9d114-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9d114-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9d114-197">committedContentVersion</span></span>|<span data-ttu-id="9d114-198">String</span><span class="sxs-lookup"><span data-stu-id="9d114-198">String</span></span>|<span data-ttu-id="9d114-199">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="9d114-199">The internal committed content version.</span></span> <span data-ttu-id="9d114-200">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="9d114-201">fileName</span><span class="sxs-lookup"><span data-stu-id="9d114-201">fileName</span></span>|<span data-ttu-id="9d114-202">String</span><span class="sxs-lookup"><span data-stu-id="9d114-202">String</span></span>|<span data-ttu-id="9d114-203">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9d114-203">The name of the main Lob application file.</span></span> <span data-ttu-id="9d114-204">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="9d114-205">size</span><span class="sxs-lookup"><span data-stu-id="9d114-205">size</span></span>|<span data-ttu-id="9d114-206">Int64</span><span class="sxs-lookup"><span data-stu-id="9d114-206">Int64</span></span>|<span data-ttu-id="9d114-207">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="9d114-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="9d114-208">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d114-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="9d114-209">packageId</span><span class="sxs-lookup"><span data-stu-id="9d114-209">packageId</span></span>|<span data-ttu-id="9d114-210">String</span><span class="sxs-lookup"><span data-stu-id="9d114-210">String</span></span>|<span data-ttu-id="9d114-211">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="9d114-211">The package identifier.</span></span>|
|<span data-ttu-id="9d114-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9d114-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9d114-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9d114-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="9d114-214">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9d114-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9d114-215">versionName</span><span class="sxs-lookup"><span data-stu-id="9d114-215">versionName</span></span>|<span data-ttu-id="9d114-216">String</span><span class="sxs-lookup"><span data-stu-id="9d114-216">String</span></span>|<span data-ttu-id="9d114-217">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="9d114-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9d114-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="9d114-218">versionCode</span></span>|<span data-ttu-id="9d114-219">String</span><span class="sxs-lookup"><span data-stu-id="9d114-219">String</span></span>|<span data-ttu-id="9d114-220">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="9d114-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="9d114-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d114-221">Response</span></span>
<span data-ttu-id="9d114-222">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9d114-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d114-223">Пример</span><span class="sxs-lookup"><span data-stu-id="9d114-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d114-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d114-224">Request</span></span>
<span data-ttu-id="9d114-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d114-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="9d114-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d114-226">Response</span></span>
<span data-ttu-id="9d114-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d114-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



