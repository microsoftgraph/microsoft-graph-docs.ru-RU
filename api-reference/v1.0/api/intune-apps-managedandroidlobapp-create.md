---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7200015c9937d604da5dfd39c74a0a556c172cbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922755"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="7bc7b-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="7bc7b-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="7bc7b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bc7b-105">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bc7b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc7b-106">Prerequisites</span></span>
<span data-ttu-id="7bc7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc7b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc7b-109">Permission type</span></span>|<span data-ttu-id="7bc7b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bc7b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bc7b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bc7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bc7b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc7b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7bc7b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bc7b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bc7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-114">Not supported.</span></span>|
|<span data-ttu-id="7bc7b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bc7b-115">Application</span></span>|<span data-ttu-id="7bc7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bc7b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bc7b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7bc7b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bc7b-118">Request headers</span></span>
|<span data-ttu-id="7bc7b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bc7b-119">Header</span></span>|<span data-ttu-id="7bc7b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7bc7b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bc7b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bc7b-121">Authorization</span></span>|<span data-ttu-id="7bc7b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7bc7b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bc7b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7bc7b-123">Accept</span></span>|<span data-ttu-id="7bc7b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7bc7b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bc7b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bc7b-125">Request body</span></span>
<span data-ttu-id="7bc7b-126">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="7bc7b-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="7bc7b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bc7b-128">Property</span></span>|<span data-ttu-id="7bc7b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7bc7b-129">Type</span></span>|<span data-ttu-id="7bc7b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7bc7b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bc7b-131">id</span><span class="sxs-lookup"><span data-stu-id="7bc7b-131">id</span></span>|<span data-ttu-id="7bc7b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7bc7b-132">String</span></span>|<span data-ttu-id="7bc7b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-133">Key of the entity.</span></span> <span data-ttu-id="7bc7b-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7bc7b-135">displayName</span></span>|<span data-ttu-id="7bc7b-136">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-136">String</span></span>|<span data-ttu-id="7bc7b-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7bc7b-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-139">описание</span><span class="sxs-lookup"><span data-stu-id="7bc7b-139">description</span></span>|<span data-ttu-id="7bc7b-140">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-140">String</span></span>|<span data-ttu-id="7bc7b-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-141">The description of the app.</span></span> <span data-ttu-id="7bc7b-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="7bc7b-143">publisher</span></span>|<span data-ttu-id="7bc7b-144">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-144">String</span></span>|<span data-ttu-id="7bc7b-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-145">The publisher of the app.</span></span> <span data-ttu-id="7bc7b-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7bc7b-147">largeIcon</span></span>|[<span data-ttu-id="7bc7b-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7bc7b-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7bc7b-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7bc7b-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bc7b-151">createdDateTime</span></span>|<span data-ttu-id="7bc7b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bc7b-152">DateTimeOffset</span></span>|<span data-ttu-id="7bc7b-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-153">The date and time the app was created.</span></span> <span data-ttu-id="7bc7b-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bc7b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="7bc7b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bc7b-156">DateTimeOffset</span></span>|<span data-ttu-id="7bc7b-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-157">The date and time the app was last modified.</span></span> <span data-ttu-id="7bc7b-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7bc7b-159">isFeatured</span></span>|<span data-ttu-id="7bc7b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bc7b-160">Boolean</span></span>|<span data-ttu-id="7bc7b-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7bc7b-162">privacyInformationUrl</span></span>|<span data-ttu-id="7bc7b-163">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-163">String</span></span>|<span data-ttu-id="7bc7b-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-164">The privacy statement Url.</span></span> <span data-ttu-id="7bc7b-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7bc7b-166">informationUrl</span></span>|<span data-ttu-id="7bc7b-167">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-167">String</span></span>|<span data-ttu-id="7bc7b-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-168">The more information Url.</span></span> <span data-ttu-id="7bc7b-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-170">owner</span><span class="sxs-lookup"><span data-stu-id="7bc7b-170">owner</span></span>|<span data-ttu-id="7bc7b-171">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-171">String</span></span>|<span data-ttu-id="7bc7b-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-172">The owner of the app.</span></span> <span data-ttu-id="7bc7b-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-174">developer</span><span class="sxs-lookup"><span data-stu-id="7bc7b-174">developer</span></span>|<span data-ttu-id="7bc7b-175">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-175">String</span></span>|<span data-ttu-id="7bc7b-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-176">The developer of the app.</span></span> <span data-ttu-id="7bc7b-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-178">notes</span><span class="sxs-lookup"><span data-stu-id="7bc7b-178">notes</span></span>|<span data-ttu-id="7bc7b-179">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-179">String</span></span>|<span data-ttu-id="7bc7b-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-180">Notes for the app.</span></span> <span data-ttu-id="7bc7b-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bc7b-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="7bc7b-182">publishingState</span></span>|[<span data-ttu-id="7bc7b-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7bc7b-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7bc7b-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-184">The publishing state for the app.</span></span> <span data-ttu-id="7bc7b-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7bc7b-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7bc7b-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7bc7b-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7bc7b-188">appAvailability</span></span>|[<span data-ttu-id="7bc7b-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="7bc7b-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="7bc7b-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-190">The Application's availability.</span></span> <span data-ttu-id="7bc7b-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="7bc7b-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7bc7b-193">version</span><span class="sxs-lookup"><span data-stu-id="7bc7b-193">version</span></span>|<span data-ttu-id="7bc7b-194">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-194">String</span></span>|<span data-ttu-id="7bc7b-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-195">The Application's version.</span></span> <span data-ttu-id="7bc7b-196">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="7bc7b-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7bc7b-197">committedContentVersion</span></span>|<span data-ttu-id="7bc7b-198">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-198">String</span></span>|<span data-ttu-id="7bc7b-199">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-199">The internal committed content version.</span></span> <span data-ttu-id="7bc7b-200">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7bc7b-201">fileName</span><span class="sxs-lookup"><span data-stu-id="7bc7b-201">fileName</span></span>|<span data-ttu-id="7bc7b-202">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-202">String</span></span>|<span data-ttu-id="7bc7b-203">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-203">The name of the main Lob application file.</span></span> <span data-ttu-id="7bc7b-204">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7bc7b-205">size</span><span class="sxs-lookup"><span data-stu-id="7bc7b-205">size</span></span>|<span data-ttu-id="7bc7b-206">Int64</span><span class="sxs-lookup"><span data-stu-id="7bc7b-206">Int64</span></span>|<span data-ttu-id="7bc7b-207">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="7bc7b-208">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bc7b-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="7bc7b-209">packageId</span><span class="sxs-lookup"><span data-stu-id="7bc7b-209">packageId</span></span>|<span data-ttu-id="7bc7b-210">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-210">String</span></span>|<span data-ttu-id="7bc7b-211">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-211">The package identifier.</span></span>|
|<span data-ttu-id="7bc7b-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7bc7b-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7bc7b-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7bc7b-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="7bc7b-214">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7bc7b-215">versionName</span><span class="sxs-lookup"><span data-stu-id="7bc7b-215">versionName</span></span>|<span data-ttu-id="7bc7b-216">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-216">String</span></span>|<span data-ttu-id="7bc7b-217">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7bc7b-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="7bc7b-218">versionCode</span></span>|<span data-ttu-id="7bc7b-219">String</span><span class="sxs-lookup"><span data-stu-id="7bc7b-219">String</span></span>|<span data-ttu-id="7bc7b-220">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="7bc7b-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bc7b-221">Response</span></span>
<span data-ttu-id="7bc7b-222">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bc7b-223">Пример</span><span class="sxs-lookup"><span data-stu-id="7bc7b-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="7bc7b-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bc7b-224">Request</span></span>
<span data-ttu-id="7bc7b-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7bc7b-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bc7b-226">Response</span></span>
<span data-ttu-id="7bc7b-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7bc7b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



