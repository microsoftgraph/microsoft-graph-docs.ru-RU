---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 095e06dc55f8528bb677051a0831ef91b82a4336
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754023"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="cdedd-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="cdedd-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="cdedd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdedd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdedd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdedd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdedd-106">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdedd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cdedd-107">Prerequisites</span></span>
<span data-ttu-id="cdedd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdedd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdedd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdedd-110">Permission type</span></span>|<span data-ttu-id="cdedd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdedd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdedd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdedd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cdedd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdedd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cdedd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdedd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdedd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdedd-115">Not supported.</span></span>|
|<span data-ttu-id="cdedd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cdedd-116">Application</span></span>|<span data-ttu-id="cdedd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdedd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdedd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdedd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="cdedd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cdedd-119">Request headers</span></span>
|<span data-ttu-id="cdedd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdedd-120">Header</span></span>|<span data-ttu-id="cdedd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cdedd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdedd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdedd-122">Authorization</span></span>|<span data-ttu-id="cdedd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdedd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdedd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cdedd-124">Accept</span></span>|<span data-ttu-id="cdedd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cdedd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdedd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdedd-126">Request body</span></span>
<span data-ttu-id="cdedd-127">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdedd-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="cdedd-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="cdedd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdedd-129">Property</span></span>|<span data-ttu-id="cdedd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cdedd-130">Type</span></span>|<span data-ttu-id="cdedd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cdedd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdedd-132">id</span><span class="sxs-lookup"><span data-stu-id="cdedd-132">id</span></span>|<span data-ttu-id="cdedd-133">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-133">String</span></span>|<span data-ttu-id="cdedd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cdedd-134">Key of the entity.</span></span> <span data-ttu-id="cdedd-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cdedd-136">displayName</span></span>|<span data-ttu-id="cdedd-137">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-137">String</span></span>|<span data-ttu-id="cdedd-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cdedd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cdedd-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-140">description</span><span class="sxs-lookup"><span data-stu-id="cdedd-140">description</span></span>|<span data-ttu-id="cdedd-141">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-141">String</span></span>|<span data-ttu-id="cdedd-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-142">The description of the app.</span></span> <span data-ttu-id="cdedd-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cdedd-144">publisher</span></span>|<span data-ttu-id="cdedd-145">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-145">String</span></span>|<span data-ttu-id="cdedd-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-146">The publisher of the app.</span></span> <span data-ttu-id="cdedd-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cdedd-148">largeIcon</span></span>|[<span data-ttu-id="cdedd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cdedd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cdedd-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cdedd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cdedd-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdedd-152">createdDateTime</span></span>|<span data-ttu-id="cdedd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdedd-153">DateTimeOffset</span></span>|<span data-ttu-id="cdedd-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-154">The date and time the app was created.</span></span> <span data-ttu-id="cdedd-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdedd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cdedd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdedd-157">DateTimeOffset</span></span>|<span data-ttu-id="cdedd-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cdedd-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cdedd-160">isFeatured</span></span>|<span data-ttu-id="cdedd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdedd-161">Boolean</span></span>|<span data-ttu-id="cdedd-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cdedd-163">privacyInformationUrl</span></span>|<span data-ttu-id="cdedd-164">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-164">String</span></span>|<span data-ttu-id="cdedd-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cdedd-165">The privacy statement Url.</span></span> <span data-ttu-id="cdedd-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cdedd-167">informationUrl</span></span>|<span data-ttu-id="cdedd-168">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-168">String</span></span>|<span data-ttu-id="cdedd-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cdedd-169">The more information Url.</span></span> <span data-ttu-id="cdedd-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-171">owner</span><span class="sxs-lookup"><span data-stu-id="cdedd-171">owner</span></span>|<span data-ttu-id="cdedd-172">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-172">String</span></span>|<span data-ttu-id="cdedd-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-173">The owner of the app.</span></span> <span data-ttu-id="cdedd-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-175">developer</span><span class="sxs-lookup"><span data-stu-id="cdedd-175">developer</span></span>|<span data-ttu-id="cdedd-176">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-176">String</span></span>|<span data-ttu-id="cdedd-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-177">The developer of the app.</span></span> <span data-ttu-id="cdedd-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-179">notes</span><span class="sxs-lookup"><span data-stu-id="cdedd-179">notes</span></span>|<span data-ttu-id="cdedd-180">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-180">String</span></span>|<span data-ttu-id="cdedd-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-181">Notes for the app.</span></span> <span data-ttu-id="cdedd-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cdedd-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="cdedd-183">publishingState</span></span>|[<span data-ttu-id="cdedd-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cdedd-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cdedd-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-185">The publishing state for the app.</span></span> <span data-ttu-id="cdedd-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cdedd-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cdedd-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cdedd-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cdedd-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cdedd-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cdedd-189">committedContentVersion</span></span>|<span data-ttu-id="cdedd-190">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-190">String</span></span>|<span data-ttu-id="cdedd-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="cdedd-191">The internal committed content version.</span></span> <span data-ttu-id="cdedd-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cdedd-193">fileName</span><span class="sxs-lookup"><span data-stu-id="cdedd-193">fileName</span></span>|<span data-ttu-id="cdedd-194">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-194">String</span></span>|<span data-ttu-id="cdedd-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-195">The name of the main Lob application file.</span></span> <span data-ttu-id="cdedd-196">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cdedd-197">size</span><span class="sxs-lookup"><span data-stu-id="cdedd-197">size</span></span>|<span data-ttu-id="cdedd-198">Int64</span><span class="sxs-lookup"><span data-stu-id="cdedd-198">Int64</span></span>|<span data-ttu-id="cdedd-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="cdedd-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="cdedd-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cdedd-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cdedd-201">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="cdedd-201">applicableArchitectures</span></span>|[<span data-ttu-id="cdedd-202">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="cdedd-202">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="cdedd-203">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cdedd-203">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="cdedd-204">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="cdedd-204">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="cdedd-205">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="cdedd-205">applicableDeviceTypes</span></span>|[<span data-ttu-id="cdedd-206">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="cdedd-206">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="cdedd-207">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cdedd-207">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="cdedd-208">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="cdedd-208">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="cdedd-209">identityName</span><span class="sxs-lookup"><span data-stu-id="cdedd-209">identityName</span></span>|<span data-ttu-id="cdedd-210">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-210">String</span></span>|<span data-ttu-id="cdedd-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-211">The Identity Name.</span></span>|
|<span data-ttu-id="cdedd-212">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="cdedd-212">identityPublisherHash</span></span>|<span data-ttu-id="cdedd-213">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-213">String</span></span>|<span data-ttu-id="cdedd-214">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="cdedd-214">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="cdedd-215">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cdedd-215">identityResourceIdentifier</span></span>|<span data-ttu-id="cdedd-216">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-216">String</span></span>|<span data-ttu-id="cdedd-217">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="cdedd-217">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="cdedd-218">isBundle</span><span class="sxs-lookup"><span data-stu-id="cdedd-218">isBundle</span></span>|<span data-ttu-id="cdedd-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdedd-219">Boolean</span></span>|<span data-ttu-id="cdedd-220">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="cdedd-220">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="cdedd-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cdedd-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cdedd-222">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cdedd-222">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="cdedd-223">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="cdedd-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cdedd-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cdedd-224">identityVersion</span></span>|<span data-ttu-id="cdedd-225">String</span><span class="sxs-lookup"><span data-stu-id="cdedd-225">String</span></span>|<span data-ttu-id="cdedd-226">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cdedd-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cdedd-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdedd-227">Response</span></span>
<span data-ttu-id="cdedd-228">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cdedd-228">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdedd-229">Пример</span><span class="sxs-lookup"><span data-stu-id="cdedd-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdedd-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdedd-230">Request</span></span>
<span data-ttu-id="cdedd-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdedd-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="cdedd-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdedd-232">Response</span></span>
<span data-ttu-id="cdedd-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdedd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```




