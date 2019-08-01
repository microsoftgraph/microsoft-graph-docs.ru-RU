---
title: Update managedAndroidLobApp
description: Обновление свойств объекта managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32ab9ae624386efd59b7824e8b900ae2ac1d2456
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002414"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="a29cd-103">Update managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="a29cd-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="a29cd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a29cd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a29cd-105">Обновление свойств объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a29cd-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a29cd-106">Prerequisites</span></span>
<span data-ttu-id="a29cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a29cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a29cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a29cd-109">Permission type</span></span>|<span data-ttu-id="a29cd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a29cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a29cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a29cd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a29cd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a29cd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a29cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a29cd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a29cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a29cd-114">Not supported.</span></span>|
|<span data-ttu-id="a29cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a29cd-115">Application</span></span>|<span data-ttu-id="a29cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a29cd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a29cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a29cd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a29cd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a29cd-118">Request headers</span></span>
|<span data-ttu-id="a29cd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a29cd-119">Header</span></span>|<span data-ttu-id="a29cd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a29cd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a29cd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a29cd-121">Authorization</span></span>|<span data-ttu-id="a29cd-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a29cd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a29cd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a29cd-123">Accept</span></span>|<span data-ttu-id="a29cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a29cd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a29cd-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a29cd-125">Request body</span></span>
<span data-ttu-id="a29cd-126">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a29cd-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="a29cd-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="a29cd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a29cd-128">Property</span></span>|<span data-ttu-id="a29cd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a29cd-129">Type</span></span>|<span data-ttu-id="a29cd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a29cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a29cd-131">id</span><span class="sxs-lookup"><span data-stu-id="a29cd-131">id</span></span>|<span data-ttu-id="a29cd-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a29cd-132">String</span></span>|<span data-ttu-id="a29cd-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a29cd-133">Key of the entity.</span></span> <span data-ttu-id="a29cd-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a29cd-135">displayName</span></span>|<span data-ttu-id="a29cd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a29cd-136">String</span></span>|<span data-ttu-id="a29cd-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a29cd-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a29cd-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-139">description</span><span class="sxs-lookup"><span data-stu-id="a29cd-139">description</span></span>|<span data-ttu-id="a29cd-140">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-140">String</span></span>|<span data-ttu-id="a29cd-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-141">The description of the app.</span></span> <span data-ttu-id="a29cd-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a29cd-143">publisher</span></span>|<span data-ttu-id="a29cd-144">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-144">String</span></span>|<span data-ttu-id="a29cd-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-145">The publisher of the app.</span></span> <span data-ttu-id="a29cd-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a29cd-147">largeIcon</span></span>|[<span data-ttu-id="a29cd-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a29cd-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a29cd-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a29cd-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a29cd-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a29cd-151">createdDateTime</span></span>|<span data-ttu-id="a29cd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a29cd-152">DateTimeOffset</span></span>|<span data-ttu-id="a29cd-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-153">The date and time the app was created.</span></span> <span data-ttu-id="a29cd-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a29cd-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a29cd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a29cd-156">DateTimeOffset</span></span>|<span data-ttu-id="a29cd-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-157">The date and time the app was last modified.</span></span> <span data-ttu-id="a29cd-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a29cd-159">isFeatured</span></span>|<span data-ttu-id="a29cd-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a29cd-160">Boolean</span></span>|<span data-ttu-id="a29cd-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a29cd-162">privacyInformationUrl</span></span>|<span data-ttu-id="a29cd-163">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-163">String</span></span>|<span data-ttu-id="a29cd-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a29cd-164">The privacy statement Url.</span></span> <span data-ttu-id="a29cd-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a29cd-166">informationUrl</span></span>|<span data-ttu-id="a29cd-167">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-167">String</span></span>|<span data-ttu-id="a29cd-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a29cd-168">The more information Url.</span></span> <span data-ttu-id="a29cd-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-170">owner</span><span class="sxs-lookup"><span data-stu-id="a29cd-170">owner</span></span>|<span data-ttu-id="a29cd-171">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-171">String</span></span>|<span data-ttu-id="a29cd-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-172">The owner of the app.</span></span> <span data-ttu-id="a29cd-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-174">developer</span><span class="sxs-lookup"><span data-stu-id="a29cd-174">developer</span></span>|<span data-ttu-id="a29cd-175">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-175">String</span></span>|<span data-ttu-id="a29cd-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-176">The developer of the app.</span></span> <span data-ttu-id="a29cd-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-178">notes</span><span class="sxs-lookup"><span data-stu-id="a29cd-178">notes</span></span>|<span data-ttu-id="a29cd-179">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-179">String</span></span>|<span data-ttu-id="a29cd-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-180">Notes for the app.</span></span> <span data-ttu-id="a29cd-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a29cd-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="a29cd-182">publishingState</span></span>|[<span data-ttu-id="a29cd-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a29cd-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a29cd-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-184">The publishing state for the app.</span></span> <span data-ttu-id="a29cd-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a29cd-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a29cd-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a29cd-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a29cd-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a29cd-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a29cd-188">appAvailability</span></span>|[<span data-ttu-id="a29cd-189">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="a29cd-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a29cd-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-190">The Application's availability.</span></span> <span data-ttu-id="a29cd-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a29cd-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="a29cd-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a29cd-193">version</span><span class="sxs-lookup"><span data-stu-id="a29cd-193">version</span></span>|<span data-ttu-id="a29cd-194">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-194">String</span></span>|<span data-ttu-id="a29cd-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-195">The Application's version.</span></span> <span data-ttu-id="a29cd-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a29cd-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a29cd-197">committedContentVersion</span></span>|<span data-ttu-id="a29cd-198">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-198">String</span></span>|<span data-ttu-id="a29cd-199">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="a29cd-199">The internal committed content version.</span></span> <span data-ttu-id="a29cd-200">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a29cd-201">fileName</span><span class="sxs-lookup"><span data-stu-id="a29cd-201">fileName</span></span>|<span data-ttu-id="a29cd-202">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-202">String</span></span>|<span data-ttu-id="a29cd-203">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="a29cd-203">The name of the main Lob application file.</span></span> <span data-ttu-id="a29cd-204">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a29cd-205">size</span><span class="sxs-lookup"><span data-stu-id="a29cd-205">size</span></span>|<span data-ttu-id="a29cd-206">Int64</span><span class="sxs-lookup"><span data-stu-id="a29cd-206">Int64</span></span>|<span data-ttu-id="a29cd-207">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="a29cd-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="a29cd-208">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a29cd-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a29cd-209">packageId</span><span class="sxs-lookup"><span data-stu-id="a29cd-209">packageId</span></span>|<span data-ttu-id="a29cd-210">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-210">String</span></span>|<span data-ttu-id="a29cd-211">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="a29cd-211">The package identifier.</span></span>|
|<span data-ttu-id="a29cd-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a29cd-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a29cd-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a29cd-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a29cd-214">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a29cd-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a29cd-215">versionName</span><span class="sxs-lookup"><span data-stu-id="a29cd-215">versionName</span></span>|<span data-ttu-id="a29cd-216">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-216">String</span></span>|<span data-ttu-id="a29cd-217">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="a29cd-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a29cd-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="a29cd-218">versionCode</span></span>|<span data-ttu-id="a29cd-219">String</span><span class="sxs-lookup"><span data-stu-id="a29cd-219">String</span></span>|<span data-ttu-id="a29cd-220">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="a29cd-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="a29cd-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="a29cd-221">Response</span></span>
<span data-ttu-id="a29cd-222">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a29cd-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a29cd-223">Пример</span><span class="sxs-lookup"><span data-stu-id="a29cd-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="a29cd-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="a29cd-224">Request</span></span>
<span data-ttu-id="a29cd-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a29cd-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a29cd-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="a29cd-226">Response</span></span>
<span data-ttu-id="a29cd-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a29cd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



