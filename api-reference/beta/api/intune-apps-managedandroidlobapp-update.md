---
title: Update managedAndroidLobApp
description: Обновление свойств объекта managedAndroidLobApp.
ms.openlocfilehash: 72cfb5ac709c7864b5a02fbfa1858eb3bb7f666b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080794"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="dd568-103">Update managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="dd568-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="dd568-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dd568-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd568-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd568-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd568-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd568-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd568-107">Обновление свойств объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd568-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dd568-108">Prerequisites</span></span>
<span data-ttu-id="dd568-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd568-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd568-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd568-111">Permission type</span></span>|<span data-ttu-id="dd568-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd568-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd568-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd568-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd568-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd568-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd568-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd568-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd568-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd568-116">Not supported.</span></span>|
|<span data-ttu-id="dd568-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd568-117">Application</span></span>|<span data-ttu-id="dd568-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd568-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd568-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd568-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dd568-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd568-120">Request headers</span></span>
|<span data-ttu-id="dd568-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd568-121">Header</span></span>|<span data-ttu-id="dd568-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd568-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd568-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd568-123">Authorization</span></span>|<span data-ttu-id="dd568-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dd568-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd568-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd568-125">Accept</span></span>|<span data-ttu-id="dd568-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd568-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd568-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd568-127">Request body</span></span>
<span data-ttu-id="dd568-128">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd568-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="dd568-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="dd568-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd568-130">Property</span></span>|<span data-ttu-id="dd568-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd568-131">Type</span></span>|<span data-ttu-id="dd568-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd568-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd568-133">id</span><span class="sxs-lookup"><span data-stu-id="dd568-133">id</span></span>|<span data-ttu-id="dd568-134">String</span><span class="sxs-lookup"><span data-stu-id="dd568-134">String</span></span>|<span data-ttu-id="dd568-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd568-135">Key of the entity.</span></span> <span data-ttu-id="dd568-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dd568-137">displayName</span></span>|<span data-ttu-id="dd568-138">String</span><span class="sxs-lookup"><span data-stu-id="dd568-138">String</span></span>|<span data-ttu-id="dd568-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="dd568-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dd568-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-141">описание</span><span class="sxs-lookup"><span data-stu-id="dd568-141">description</span></span>|<span data-ttu-id="dd568-142">String</span><span class="sxs-lookup"><span data-stu-id="dd568-142">String</span></span>|<span data-ttu-id="dd568-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-143">The description of the app.</span></span> <span data-ttu-id="dd568-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-145">publisher</span><span class="sxs-lookup"><span data-stu-id="dd568-145">publisher</span></span>|<span data-ttu-id="dd568-146">String</span><span class="sxs-lookup"><span data-stu-id="dd568-146">String</span></span>|<span data-ttu-id="dd568-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-147">The publisher of the app.</span></span> <span data-ttu-id="dd568-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dd568-149">largeIcon</span></span>|[<span data-ttu-id="dd568-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dd568-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dd568-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="dd568-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dd568-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd568-153">createdDateTime</span></span>|<span data-ttu-id="dd568-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd568-154">DateTimeOffset</span></span>|<span data-ttu-id="dd568-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-155">The date and time the app was created.</span></span> <span data-ttu-id="dd568-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd568-157">lastModifiedDateTime</span></span>|<span data-ttu-id="dd568-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd568-158">DateTimeOffset</span></span>|<span data-ttu-id="dd568-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-159">The date and time the app was last modified.</span></span> <span data-ttu-id="dd568-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dd568-161">isFeatured</span></span>|<span data-ttu-id="dd568-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd568-162">Boolean</span></span>|<span data-ttu-id="dd568-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dd568-164">privacyInformationUrl</span></span>|<span data-ttu-id="dd568-165">String</span><span class="sxs-lookup"><span data-stu-id="dd568-165">String</span></span>|<span data-ttu-id="dd568-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="dd568-166">The privacy statement Url.</span></span> <span data-ttu-id="dd568-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dd568-168">informationUrl</span></span>|<span data-ttu-id="dd568-169">String</span><span class="sxs-lookup"><span data-stu-id="dd568-169">String</span></span>|<span data-ttu-id="dd568-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="dd568-170">The more information Url.</span></span> <span data-ttu-id="dd568-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-172">owner</span><span class="sxs-lookup"><span data-stu-id="dd568-172">owner</span></span>|<span data-ttu-id="dd568-173">String</span><span class="sxs-lookup"><span data-stu-id="dd568-173">String</span></span>|<span data-ttu-id="dd568-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-174">The owner of the app.</span></span> <span data-ttu-id="dd568-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-176">developer</span><span class="sxs-lookup"><span data-stu-id="dd568-176">developer</span></span>|<span data-ttu-id="dd568-177">String</span><span class="sxs-lookup"><span data-stu-id="dd568-177">String</span></span>|<span data-ttu-id="dd568-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-178">The developer of the app.</span></span> <span data-ttu-id="dd568-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-180">notes</span><span class="sxs-lookup"><span data-stu-id="dd568-180">notes</span></span>|<span data-ttu-id="dd568-181">String</span><span class="sxs-lookup"><span data-stu-id="dd568-181">String</span></span>|<span data-ttu-id="dd568-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="dd568-182">Notes for the app.</span></span> <span data-ttu-id="dd568-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="dd568-184">uploadState</span></span>|<span data-ttu-id="dd568-185">Int32</span><span class="sxs-lookup"><span data-stu-id="dd568-185">Int32</span></span>|<span data-ttu-id="dd568-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="dd568-186">The upload state.</span></span> <span data-ttu-id="dd568-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd568-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="dd568-188">publishingState</span></span>|[<span data-ttu-id="dd568-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dd568-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dd568-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-190">The publishing state for the app.</span></span> <span data-ttu-id="dd568-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="dd568-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dd568-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dd568-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dd568-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dd568-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="dd568-194">appAvailability</span></span>|[<span data-ttu-id="dd568-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="dd568-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="dd568-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-196">The Application's availability.</span></span> <span data-ttu-id="dd568-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="dd568-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="dd568-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="dd568-199">version</span><span class="sxs-lookup"><span data-stu-id="dd568-199">version</span></span>|<span data-ttu-id="dd568-200">String</span><span class="sxs-lookup"><span data-stu-id="dd568-200">String</span></span>|<span data-ttu-id="dd568-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-201">The Application's version.</span></span> <span data-ttu-id="dd568-202">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="dd568-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dd568-203">committedContentVersion</span></span>|<span data-ttu-id="dd568-204">String</span><span class="sxs-lookup"><span data-stu-id="dd568-204">String</span></span>|<span data-ttu-id="dd568-205">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="dd568-205">The internal committed content version.</span></span> <span data-ttu-id="dd568-206">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dd568-207">fileName</span><span class="sxs-lookup"><span data-stu-id="dd568-207">fileName</span></span>|<span data-ttu-id="dd568-208">String</span><span class="sxs-lookup"><span data-stu-id="dd568-208">String</span></span>|<span data-ttu-id="dd568-209">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="dd568-209">The name of the main Lob application file.</span></span> <span data-ttu-id="dd568-210">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dd568-211">size</span><span class="sxs-lookup"><span data-stu-id="dd568-211">size</span></span>|<span data-ttu-id="dd568-212">Int64</span><span class="sxs-lookup"><span data-stu-id="dd568-212">Int64</span></span>|<span data-ttu-id="dd568-213">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="dd568-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="dd568-214">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="dd568-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dd568-215">packageId</span><span class="sxs-lookup"><span data-stu-id="dd568-215">packageId</span></span>|<span data-ttu-id="dd568-216">String</span><span class="sxs-lookup"><span data-stu-id="dd568-216">String</span></span>|<span data-ttu-id="dd568-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="dd568-217">The package identifier.</span></span>|
|<span data-ttu-id="dd568-218">identityName</span><span class="sxs-lookup"><span data-stu-id="dd568-218">identityName</span></span>|<span data-ttu-id="dd568-219">String</span><span class="sxs-lookup"><span data-stu-id="dd568-219">String</span></span>|<span data-ttu-id="dd568-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dd568-220">The Identity Name.</span></span>|
|<span data-ttu-id="dd568-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd568-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dd568-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd568-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="dd568-223">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="dd568-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dd568-224">versionName</span><span class="sxs-lookup"><span data-stu-id="dd568-224">versionName</span></span>|<span data-ttu-id="dd568-225">String</span><span class="sxs-lookup"><span data-stu-id="dd568-225">String</span></span>|<span data-ttu-id="dd568-226">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="dd568-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dd568-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="dd568-227">versionCode</span></span>|<span data-ttu-id="dd568-228">String</span><span class="sxs-lookup"><span data-stu-id="dd568-228">String</span></span>|<span data-ttu-id="dd568-229">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="dd568-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dd568-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="dd568-230">identityVersion</span></span>|<span data-ttu-id="dd568-231">String</span><span class="sxs-lookup"><span data-stu-id="dd568-231">String</span></span>|<span data-ttu-id="dd568-232">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="dd568-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="dd568-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd568-233">Response</span></span>
<span data-ttu-id="dd568-234">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dd568-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd568-235">Пример</span><span class="sxs-lookup"><span data-stu-id="dd568-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd568-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd568-236">Request</span></span>
<span data-ttu-id="dd568-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd568-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1384

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="dd568-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd568-238">Response</span></span>
<span data-ttu-id="dd568-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="dd568-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1551

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
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





