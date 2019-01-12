---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cff6787f782c4c86cbcc9298c0205e75315614dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950902"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="914e7-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="914e7-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="914e7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="914e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="914e7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="914e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="914e7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="914e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="914e7-107">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="914e7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="914e7-108">Prerequisites</span></span>
<span data-ttu-id="914e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="914e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="914e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="914e7-111">Permission type</span></span>|<span data-ttu-id="914e7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="914e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="914e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="914e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="914e7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="914e7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="914e7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="914e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="914e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="914e7-116">Not supported.</span></span>|
|<span data-ttu-id="914e7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="914e7-117">Application</span></span>|<span data-ttu-id="914e7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="914e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="914e7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="914e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="914e7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="914e7-120">Request headers</span></span>
|<span data-ttu-id="914e7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="914e7-121">Header</span></span>|<span data-ttu-id="914e7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="914e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="914e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="914e7-123">Authorization</span></span>|<span data-ttu-id="914e7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="914e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="914e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="914e7-125">Accept</span></span>|<span data-ttu-id="914e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="914e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="914e7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="914e7-127">Request body</span></span>
<span data-ttu-id="914e7-128">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="914e7-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="914e7-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="914e7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="914e7-130">Property</span></span>|<span data-ttu-id="914e7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="914e7-131">Type</span></span>|<span data-ttu-id="914e7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="914e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914e7-133">id</span><span class="sxs-lookup"><span data-stu-id="914e7-133">id</span></span>|<span data-ttu-id="914e7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="914e7-134">String</span></span>|<span data-ttu-id="914e7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="914e7-135">Key of the entity.</span></span> <span data-ttu-id="914e7-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="914e7-137">displayName</span></span>|<span data-ttu-id="914e7-138">String</span><span class="sxs-lookup"><span data-stu-id="914e7-138">String</span></span>|<span data-ttu-id="914e7-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="914e7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="914e7-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-141">описание</span><span class="sxs-lookup"><span data-stu-id="914e7-141">description</span></span>|<span data-ttu-id="914e7-142">String</span><span class="sxs-lookup"><span data-stu-id="914e7-142">String</span></span>|<span data-ttu-id="914e7-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-143">The description of the app.</span></span> <span data-ttu-id="914e7-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="914e7-145">publisher</span></span>|<span data-ttu-id="914e7-146">String</span><span class="sxs-lookup"><span data-stu-id="914e7-146">String</span></span>|<span data-ttu-id="914e7-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-147">The publisher of the app.</span></span> <span data-ttu-id="914e7-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="914e7-149">largeIcon</span></span>|[<span data-ttu-id="914e7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="914e7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="914e7-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="914e7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="914e7-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="914e7-153">createdDateTime</span></span>|<span data-ttu-id="914e7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914e7-154">DateTimeOffset</span></span>|<span data-ttu-id="914e7-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-155">The date and time the app was created.</span></span> <span data-ttu-id="914e7-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="914e7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="914e7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="914e7-158">DateTimeOffset</span></span>|<span data-ttu-id="914e7-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="914e7-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="914e7-161">isFeatured</span></span>|<span data-ttu-id="914e7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="914e7-162">Boolean</span></span>|<span data-ttu-id="914e7-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="914e7-164">privacyInformationUrl</span></span>|<span data-ttu-id="914e7-165">String</span><span class="sxs-lookup"><span data-stu-id="914e7-165">String</span></span>|<span data-ttu-id="914e7-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="914e7-166">The privacy statement Url.</span></span> <span data-ttu-id="914e7-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="914e7-168">informationUrl</span></span>|<span data-ttu-id="914e7-169">String</span><span class="sxs-lookup"><span data-stu-id="914e7-169">String</span></span>|<span data-ttu-id="914e7-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="914e7-170">The more information Url.</span></span> <span data-ttu-id="914e7-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-172">owner</span><span class="sxs-lookup"><span data-stu-id="914e7-172">owner</span></span>|<span data-ttu-id="914e7-173">String</span><span class="sxs-lookup"><span data-stu-id="914e7-173">String</span></span>|<span data-ttu-id="914e7-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-174">The owner of the app.</span></span> <span data-ttu-id="914e7-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-176">developer</span><span class="sxs-lookup"><span data-stu-id="914e7-176">developer</span></span>|<span data-ttu-id="914e7-177">String</span><span class="sxs-lookup"><span data-stu-id="914e7-177">String</span></span>|<span data-ttu-id="914e7-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-178">The developer of the app.</span></span> <span data-ttu-id="914e7-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-180">notes</span><span class="sxs-lookup"><span data-stu-id="914e7-180">notes</span></span>|<span data-ttu-id="914e7-181">String</span><span class="sxs-lookup"><span data-stu-id="914e7-181">String</span></span>|<span data-ttu-id="914e7-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="914e7-182">Notes for the app.</span></span> <span data-ttu-id="914e7-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="914e7-184">uploadState</span></span>|<span data-ttu-id="914e7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="914e7-185">Int32</span></span>|<span data-ttu-id="914e7-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="914e7-186">The upload state.</span></span> <span data-ttu-id="914e7-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="914e7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="914e7-188">publishingState</span></span>|[<span data-ttu-id="914e7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="914e7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="914e7-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-190">The publishing state for the app.</span></span> <span data-ttu-id="914e7-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="914e7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="914e7-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="914e7-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="914e7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="914e7-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="914e7-194">committedContentVersion</span></span>|<span data-ttu-id="914e7-195">String</span><span class="sxs-lookup"><span data-stu-id="914e7-195">String</span></span>|<span data-ttu-id="914e7-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="914e7-196">The internal committed content version.</span></span> <span data-ttu-id="914e7-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="914e7-198">fileName</span><span class="sxs-lookup"><span data-stu-id="914e7-198">fileName</span></span>|<span data-ttu-id="914e7-199">String</span><span class="sxs-lookup"><span data-stu-id="914e7-199">String</span></span>|<span data-ttu-id="914e7-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-200">The name of the main Lob application file.</span></span> <span data-ttu-id="914e7-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="914e7-202">size</span><span class="sxs-lookup"><span data-stu-id="914e7-202">size</span></span>|<span data-ttu-id="914e7-203">Int64</span><span class="sxs-lookup"><span data-stu-id="914e7-203">Int64</span></span>|<span data-ttu-id="914e7-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="914e7-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="914e7-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="914e7-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="914e7-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="914e7-206">commandLine</span></span>|<span data-ttu-id="914e7-207">String</span><span class="sxs-lookup"><span data-stu-id="914e7-207">String</span></span>|<span data-ttu-id="914e7-208">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="914e7-208">The command line.</span></span>|
|<span data-ttu-id="914e7-209">productCode</span><span class="sxs-lookup"><span data-stu-id="914e7-209">productCode</span></span>|<span data-ttu-id="914e7-210">String</span><span class="sxs-lookup"><span data-stu-id="914e7-210">String</span></span>|<span data-ttu-id="914e7-211">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="914e7-211">The product code.</span></span>|
|<span data-ttu-id="914e7-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="914e7-212">productVersion</span></span>|<span data-ttu-id="914e7-213">String</span><span class="sxs-lookup"><span data-stu-id="914e7-213">String</span></span>|<span data-ttu-id="914e7-214">Версия бизнес-приложения MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="914e7-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="914e7-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="914e7-215">ignoreVersionDetection</span></span>|<span data-ttu-id="914e7-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="914e7-216">Boolean</span></span>|<span data-ttu-id="914e7-217">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="914e7-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="914e7-218">Для бизнес-приложений MSI Windows Mobile с функцией самостоятельного обновления следует использовать значение true.</span><span class="sxs-lookup"><span data-stu-id="914e7-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="914e7-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="914e7-219">identityVersion</span></span>|<span data-ttu-id="914e7-220">String</span><span class="sxs-lookup"><span data-stu-id="914e7-220">String</span></span>|<span data-ttu-id="914e7-221">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="914e7-221">The identity version.</span></span>|
|<span data-ttu-id="914e7-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="914e7-222">useDeviceContext</span></span>|<span data-ttu-id="914e7-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="914e7-223">Boolean</span></span>|<span data-ttu-id="914e7-224">Указывает, следует ли установить MSI двумя режимами в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="914e7-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="914e7-225">Если значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="914e7-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="914e7-226">Если задано значение false, приложение будет установлено для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="914e7-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="914e7-227">Если значение null, служба будет использовать пакет MSI контекст установки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="914e7-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="914e7-228">В случае MSI двумя режимами это значение по умолчанию будет пользователя.</span><span class="sxs-lookup"><span data-stu-id="914e7-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="914e7-229">Не могут задаваться для приложений двумя режимами.</span><span class="sxs-lookup"><span data-stu-id="914e7-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="914e7-230">Нельзя изменить после первоначального создания приложения.</span><span class="sxs-lookup"><span data-stu-id="914e7-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="914e7-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="914e7-231">Response</span></span>
<span data-ttu-id="914e7-232">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="914e7-232">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="914e7-233">Пример</span><span class="sxs-lookup"><span data-stu-id="914e7-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="914e7-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="914e7-234">Request</span></span>
<span data-ttu-id="914e7-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="914e7-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 963

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="914e7-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="914e7-236">Response</span></span>
<span data-ttu-id="914e7-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="914e7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```





