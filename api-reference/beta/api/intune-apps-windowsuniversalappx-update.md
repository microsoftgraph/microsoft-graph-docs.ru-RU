---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b47da8672b980b30471f87bbbe4d9cee14eb5089
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892521"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="40fcb-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="40fcb-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="40fcb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40fcb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40fcb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40fcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40fcb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40fcb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40fcb-107">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-107">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40fcb-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="40fcb-108">Prerequisites</span></span>
<span data-ttu-id="40fcb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40fcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40fcb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40fcb-111">Permission type</span></span>|<span data-ttu-id="40fcb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40fcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40fcb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40fcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40fcb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40fcb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40fcb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40fcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40fcb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40fcb-116">Not supported.</span></span>|
|<span data-ttu-id="40fcb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40fcb-117">Application</span></span>|<span data-ttu-id="40fcb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40fcb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40fcb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40fcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="40fcb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40fcb-120">Request headers</span></span>
|<span data-ttu-id="40fcb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40fcb-121">Header</span></span>|<span data-ttu-id="40fcb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40fcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40fcb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40fcb-123">Authorization</span></span>|<span data-ttu-id="40fcb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="40fcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40fcb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40fcb-125">Accept</span></span>|<span data-ttu-id="40fcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40fcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40fcb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40fcb-127">Request body</span></span>
<span data-ttu-id="40fcb-128">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40fcb-128">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="40fcb-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-129">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="40fcb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="40fcb-130">Property</span></span>|<span data-ttu-id="40fcb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40fcb-131">Type</span></span>|<span data-ttu-id="40fcb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40fcb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40fcb-133">id</span><span class="sxs-lookup"><span data-stu-id="40fcb-133">id</span></span>|<span data-ttu-id="40fcb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="40fcb-134">String</span></span>|<span data-ttu-id="40fcb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="40fcb-135">Key of the entity.</span></span> <span data-ttu-id="40fcb-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="40fcb-137">displayName</span></span>|<span data-ttu-id="40fcb-138">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-138">String</span></span>|<span data-ttu-id="40fcb-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="40fcb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="40fcb-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-141">описание</span><span class="sxs-lookup"><span data-stu-id="40fcb-141">description</span></span>|<span data-ttu-id="40fcb-142">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-142">String</span></span>|<span data-ttu-id="40fcb-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-143">The description of the app.</span></span> <span data-ttu-id="40fcb-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="40fcb-145">publisher</span></span>|<span data-ttu-id="40fcb-146">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-146">String</span></span>|<span data-ttu-id="40fcb-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-147">The publisher of the app.</span></span> <span data-ttu-id="40fcb-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="40fcb-149">largeIcon</span></span>|[<span data-ttu-id="40fcb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="40fcb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="40fcb-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="40fcb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="40fcb-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40fcb-153">createdDateTime</span></span>|<span data-ttu-id="40fcb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40fcb-154">DateTimeOffset</span></span>|<span data-ttu-id="40fcb-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-155">The date and time the app was created.</span></span> <span data-ttu-id="40fcb-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40fcb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="40fcb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40fcb-158">DateTimeOffset</span></span>|<span data-ttu-id="40fcb-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="40fcb-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="40fcb-161">isFeatured</span></span>|<span data-ttu-id="40fcb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="40fcb-162">Boolean</span></span>|<span data-ttu-id="40fcb-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="40fcb-164">privacyInformationUrl</span></span>|<span data-ttu-id="40fcb-165">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-165">String</span></span>|<span data-ttu-id="40fcb-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="40fcb-166">The privacy statement Url.</span></span> <span data-ttu-id="40fcb-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="40fcb-168">informationUrl</span></span>|<span data-ttu-id="40fcb-169">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-169">String</span></span>|<span data-ttu-id="40fcb-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="40fcb-170">The more information Url.</span></span> <span data-ttu-id="40fcb-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-172">owner</span><span class="sxs-lookup"><span data-stu-id="40fcb-172">owner</span></span>|<span data-ttu-id="40fcb-173">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-173">String</span></span>|<span data-ttu-id="40fcb-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-174">The owner of the app.</span></span> <span data-ttu-id="40fcb-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-176">developer</span><span class="sxs-lookup"><span data-stu-id="40fcb-176">developer</span></span>|<span data-ttu-id="40fcb-177">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-177">String</span></span>|<span data-ttu-id="40fcb-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-178">The developer of the app.</span></span> <span data-ttu-id="40fcb-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-180">notes</span><span class="sxs-lookup"><span data-stu-id="40fcb-180">notes</span></span>|<span data-ttu-id="40fcb-181">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-181">String</span></span>|<span data-ttu-id="40fcb-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="40fcb-182">Notes for the app.</span></span> <span data-ttu-id="40fcb-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="40fcb-184">uploadState</span></span>|<span data-ttu-id="40fcb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="40fcb-185">Int32</span></span>|<span data-ttu-id="40fcb-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="40fcb-186">The upload state.</span></span> <span data-ttu-id="40fcb-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40fcb-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="40fcb-188">publishingState</span></span>|[<span data-ttu-id="40fcb-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="40fcb-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="40fcb-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-190">The publishing state for the app.</span></span> <span data-ttu-id="40fcb-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="40fcb-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="40fcb-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="40fcb-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="40fcb-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="40fcb-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="40fcb-194">committedContentVersion</span></span>|<span data-ttu-id="40fcb-195">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-195">String</span></span>|<span data-ttu-id="40fcb-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="40fcb-196">The internal committed content version.</span></span> <span data-ttu-id="40fcb-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="40fcb-198">fileName</span><span class="sxs-lookup"><span data-stu-id="40fcb-198">fileName</span></span>|<span data-ttu-id="40fcb-199">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-199">String</span></span>|<span data-ttu-id="40fcb-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-200">The name of the main Lob application file.</span></span> <span data-ttu-id="40fcb-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="40fcb-202">size</span><span class="sxs-lookup"><span data-stu-id="40fcb-202">size</span></span>|<span data-ttu-id="40fcb-203">Int64</span><span class="sxs-lookup"><span data-stu-id="40fcb-203">Int64</span></span>|<span data-ttu-id="40fcb-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="40fcb-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="40fcb-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40fcb-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="40fcb-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="40fcb-206">applicableArchitectures</span></span>|[<span data-ttu-id="40fcb-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="40fcb-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="40fcb-208">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="40fcb-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="40fcb-209">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="40fcb-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="40fcb-210">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="40fcb-210">applicableDeviceTypes</span></span>|[<span data-ttu-id="40fcb-211">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="40fcb-211">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="40fcb-212">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="40fcb-212">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="40fcb-213">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="40fcb-213">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="40fcb-214">identityName</span><span class="sxs-lookup"><span data-stu-id="40fcb-214">identityName</span></span>|<span data-ttu-id="40fcb-215">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-215">String</span></span>|<span data-ttu-id="40fcb-216">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-216">The Identity Name.</span></span>|
|<span data-ttu-id="40fcb-217">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="40fcb-217">identityPublisherHash</span></span>|<span data-ttu-id="40fcb-218">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-218">String</span></span>|<span data-ttu-id="40fcb-219">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="40fcb-219">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="40fcb-220">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="40fcb-220">identityResourceIdentifier</span></span>|<span data-ttu-id="40fcb-221">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-221">String</span></span>|<span data-ttu-id="40fcb-222">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="40fcb-222">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="40fcb-223">isBundle</span><span class="sxs-lookup"><span data-stu-id="40fcb-223">isBundle</span></span>|<span data-ttu-id="40fcb-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="40fcb-224">Boolean</span></span>|<span data-ttu-id="40fcb-225">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="40fcb-225">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="40fcb-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40fcb-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="40fcb-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40fcb-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="40fcb-228">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="40fcb-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="40fcb-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="40fcb-229">identityVersion</span></span>|<span data-ttu-id="40fcb-230">String</span><span class="sxs-lookup"><span data-stu-id="40fcb-230">String</span></span>|<span data-ttu-id="40fcb-231">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="40fcb-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="40fcb-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="40fcb-232">Response</span></span>
<span data-ttu-id="40fcb-233">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="40fcb-233">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40fcb-234">Пример</span><span class="sxs-lookup"><span data-stu-id="40fcb-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="40fcb-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="40fcb-235">Request</span></span>
<span data-ttu-id="40fcb-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40fcb-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1308

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
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="40fcb-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="40fcb-237">Response</span></span>
<span data-ttu-id="40fcb-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40fcb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1475

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
  "uploadState": 11,
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
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```





