---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82a3a3b1b9e767e0fe8cb93b6c2380896ae22851
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939968"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="c62e5-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="c62e5-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="c62e5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c62e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c62e5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c62e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c62e5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c62e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c62e5-107">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c62e5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c62e5-108">Prerequisites</span></span>
<span data-ttu-id="c62e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c62e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c62e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c62e5-111">Permission type</span></span>|<span data-ttu-id="c62e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c62e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c62e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c62e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c62e5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c62e5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c62e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c62e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c62e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c62e5-116">Not supported.</span></span>|
|<span data-ttu-id="c62e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c62e5-117">Application</span></span>|<span data-ttu-id="c62e5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c62e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c62e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c62e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c62e5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c62e5-120">Request headers</span></span>
|<span data-ttu-id="c62e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c62e5-121">Header</span></span>|<span data-ttu-id="c62e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c62e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c62e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c62e5-123">Authorization</span></span>|<span data-ttu-id="c62e5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c62e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c62e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c62e5-125">Accept</span></span>|<span data-ttu-id="c62e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c62e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c62e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c62e5-127">Request body</span></span>
<span data-ttu-id="c62e5-128">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c62e5-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="c62e5-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="c62e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c62e5-130">Property</span></span>|<span data-ttu-id="c62e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c62e5-131">Type</span></span>|<span data-ttu-id="c62e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c62e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c62e5-133">id</span><span class="sxs-lookup"><span data-stu-id="c62e5-133">id</span></span>|<span data-ttu-id="c62e5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c62e5-134">String</span></span>|<span data-ttu-id="c62e5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c62e5-135">Key of the entity.</span></span> <span data-ttu-id="c62e5-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c62e5-137">displayName</span></span>|<span data-ttu-id="c62e5-138">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-138">String</span></span>|<span data-ttu-id="c62e5-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c62e5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c62e5-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-141">описание</span><span class="sxs-lookup"><span data-stu-id="c62e5-141">description</span></span>|<span data-ttu-id="c62e5-142">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-142">String</span></span>|<span data-ttu-id="c62e5-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-143">The description of the app.</span></span> <span data-ttu-id="c62e5-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c62e5-145">publisher</span></span>|<span data-ttu-id="c62e5-146">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-146">String</span></span>|<span data-ttu-id="c62e5-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-147">The publisher of the app.</span></span> <span data-ttu-id="c62e5-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c62e5-149">largeIcon</span></span>|[<span data-ttu-id="c62e5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c62e5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c62e5-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c62e5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c62e5-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c62e5-153">createdDateTime</span></span>|<span data-ttu-id="c62e5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c62e5-154">DateTimeOffset</span></span>|<span data-ttu-id="c62e5-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-155">The date and time the app was created.</span></span> <span data-ttu-id="c62e5-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c62e5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c62e5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c62e5-158">DateTimeOffset</span></span>|<span data-ttu-id="c62e5-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c62e5-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c62e5-161">isFeatured</span></span>|<span data-ttu-id="c62e5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c62e5-162">Boolean</span></span>|<span data-ttu-id="c62e5-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c62e5-164">privacyInformationUrl</span></span>|<span data-ttu-id="c62e5-165">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-165">String</span></span>|<span data-ttu-id="c62e5-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c62e5-166">The privacy statement Url.</span></span> <span data-ttu-id="c62e5-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c62e5-168">informationUrl</span></span>|<span data-ttu-id="c62e5-169">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-169">String</span></span>|<span data-ttu-id="c62e5-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c62e5-170">The more information Url.</span></span> <span data-ttu-id="c62e5-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-172">owner</span><span class="sxs-lookup"><span data-stu-id="c62e5-172">owner</span></span>|<span data-ttu-id="c62e5-173">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-173">String</span></span>|<span data-ttu-id="c62e5-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-174">The owner of the app.</span></span> <span data-ttu-id="c62e5-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-176">developer</span><span class="sxs-lookup"><span data-stu-id="c62e5-176">developer</span></span>|<span data-ttu-id="c62e5-177">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-177">String</span></span>|<span data-ttu-id="c62e5-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-178">The developer of the app.</span></span> <span data-ttu-id="c62e5-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-180">notes</span><span class="sxs-lookup"><span data-stu-id="c62e5-180">notes</span></span>|<span data-ttu-id="c62e5-181">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-181">String</span></span>|<span data-ttu-id="c62e5-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="c62e5-182">Notes for the app.</span></span> <span data-ttu-id="c62e5-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c62e5-184">uploadState</span></span>|<span data-ttu-id="c62e5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c62e5-185">Int32</span></span>|<span data-ttu-id="c62e5-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="c62e5-186">The upload state.</span></span> <span data-ttu-id="c62e5-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c62e5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c62e5-188">publishingState</span></span>|[<span data-ttu-id="c62e5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c62e5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c62e5-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-190">The publishing state for the app.</span></span> <span data-ttu-id="c62e5-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c62e5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c62e5-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c62e5-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c62e5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c62e5-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c62e5-194">appAvailability</span></span>|[<span data-ttu-id="c62e5-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c62e5-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c62e5-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-196">The Application's availability.</span></span> <span data-ttu-id="c62e5-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c62e5-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c62e5-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c62e5-199">version</span><span class="sxs-lookup"><span data-stu-id="c62e5-199">version</span></span>|<span data-ttu-id="c62e5-200">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-200">String</span></span>|<span data-ttu-id="c62e5-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-201">The Application's version.</span></span> <span data-ttu-id="c62e5-202">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c62e5-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c62e5-203">committedContentVersion</span></span>|<span data-ttu-id="c62e5-204">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-204">String</span></span>|<span data-ttu-id="c62e5-205">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="c62e5-205">The internal committed content version.</span></span> <span data-ttu-id="c62e5-206">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c62e5-207">fileName</span><span class="sxs-lookup"><span data-stu-id="c62e5-207">fileName</span></span>|<span data-ttu-id="c62e5-208">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-208">String</span></span>|<span data-ttu-id="c62e5-209">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-209">The name of the main Lob application file.</span></span> <span data-ttu-id="c62e5-210">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c62e5-211">size</span><span class="sxs-lookup"><span data-stu-id="c62e5-211">size</span></span>|<span data-ttu-id="c62e5-212">Int64</span><span class="sxs-lookup"><span data-stu-id="c62e5-212">Int64</span></span>|<span data-ttu-id="c62e5-213">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="c62e5-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="c62e5-214">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c62e5-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c62e5-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="c62e5-215">bundleId</span></span>|<span data-ttu-id="c62e5-216">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-216">String</span></span>|<span data-ttu-id="c62e5-217">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-217">The Identity Name.</span></span>|
|<span data-ttu-id="c62e5-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="c62e5-218">applicableDeviceType</span></span>|[<span data-ttu-id="c62e5-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c62e5-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="c62e5-220">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="c62e5-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="c62e5-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c62e5-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c62e5-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c62e5-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="c62e5-223">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c62e5-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c62e5-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c62e5-224">expirationDateTime</span></span>|<span data-ttu-id="c62e5-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c62e5-225">DateTimeOffset</span></span>|<span data-ttu-id="c62e5-226">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="c62e5-226">The expiration time.</span></span>|
|<span data-ttu-id="c62e5-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="c62e5-227">versionNumber</span></span>|<span data-ttu-id="c62e5-228">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-228">String</span></span>|<span data-ttu-id="c62e5-229">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="c62e5-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c62e5-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="c62e5-230">buildNumber</span></span>|<span data-ttu-id="c62e5-231">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-231">String</span></span>|<span data-ttu-id="c62e5-232">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="c62e5-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c62e5-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c62e5-233">identityVersion</span></span>|<span data-ttu-id="c62e5-234">String</span><span class="sxs-lookup"><span data-stu-id="c62e5-234">String</span></span>|<span data-ttu-id="c62e5-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c62e5-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c62e5-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="c62e5-236">Response</span></span>
<span data-ttu-id="c62e5-237">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c62e5-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c62e5-238">Пример</span><span class="sxs-lookup"><span data-stu-id="c62e5-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="c62e5-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="c62e5-239">Request</span></span>
<span data-ttu-id="c62e5-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c62e5-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1366

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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="c62e5-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="c62e5-241">Response</span></span>
<span data-ttu-id="c62e5-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c62e5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1529

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
  "uploadState": 11,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





