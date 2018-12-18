---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
author: tfitzmac
ms.openlocfilehash: 859d32fbf053ba22c0bd59afe8ad24d6b05c84a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310747"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="48423-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="48423-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="48423-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48423-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48423-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48423-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48423-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48423-107">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="48423-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48423-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48423-108">Prerequisites</span></span>
<span data-ttu-id="48423-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48423-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48423-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48423-111">Permission type</span></span>|<span data-ttu-id="48423-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48423-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48423-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48423-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48423-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48423-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48423-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48423-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48423-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48423-116">Not supported.</span></span>|
|<span data-ttu-id="48423-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48423-117">Application</span></span>|<span data-ttu-id="48423-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48423-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48423-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48423-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="48423-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48423-120">Request headers</span></span>
|<span data-ttu-id="48423-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48423-121">Header</span></span>|<span data-ttu-id="48423-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48423-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48423-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48423-123">Authorization</span></span>|<span data-ttu-id="48423-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48423-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48423-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48423-125">Accept</span></span>|<span data-ttu-id="48423-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48423-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48423-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48423-127">Request body</span></span>
<span data-ttu-id="48423-128">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48423-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="48423-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="48423-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="48423-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48423-130">Property</span></span>|<span data-ttu-id="48423-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48423-131">Type</span></span>|<span data-ttu-id="48423-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48423-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48423-133">id</span><span class="sxs-lookup"><span data-stu-id="48423-133">id</span></span>|<span data-ttu-id="48423-134">Строка</span><span class="sxs-lookup"><span data-stu-id="48423-134">String</span></span>|<span data-ttu-id="48423-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48423-135">Key of the entity.</span></span> <span data-ttu-id="48423-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-137">displayName</span><span class="sxs-lookup"><span data-stu-id="48423-137">displayName</span></span>|<span data-ttu-id="48423-138">String</span><span class="sxs-lookup"><span data-stu-id="48423-138">String</span></span>|<span data-ttu-id="48423-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="48423-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="48423-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-141">описание</span><span class="sxs-lookup"><span data-stu-id="48423-141">description</span></span>|<span data-ttu-id="48423-142">String</span><span class="sxs-lookup"><span data-stu-id="48423-142">String</span></span>|<span data-ttu-id="48423-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-143">The description of the app.</span></span> <span data-ttu-id="48423-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-145">publisher</span><span class="sxs-lookup"><span data-stu-id="48423-145">publisher</span></span>|<span data-ttu-id="48423-146">String</span><span class="sxs-lookup"><span data-stu-id="48423-146">String</span></span>|<span data-ttu-id="48423-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-147">The publisher of the app.</span></span> <span data-ttu-id="48423-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48423-149">largeIcon</span></span>|[<span data-ttu-id="48423-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48423-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48423-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="48423-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="48423-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48423-153">createdDateTime</span></span>|<span data-ttu-id="48423-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48423-154">DateTimeOffset</span></span>|<span data-ttu-id="48423-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-155">The date and time the app was created.</span></span> <span data-ttu-id="48423-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48423-157">lastModifiedDateTime</span></span>|<span data-ttu-id="48423-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48423-158">DateTimeOffset</span></span>|<span data-ttu-id="48423-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-159">The date and time the app was last modified.</span></span> <span data-ttu-id="48423-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48423-161">isFeatured</span></span>|<span data-ttu-id="48423-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="48423-162">Boolean</span></span>|<span data-ttu-id="48423-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48423-164">privacyInformationUrl</span></span>|<span data-ttu-id="48423-165">String</span><span class="sxs-lookup"><span data-stu-id="48423-165">String</span></span>|<span data-ttu-id="48423-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="48423-166">The privacy statement Url.</span></span> <span data-ttu-id="48423-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48423-168">informationUrl</span></span>|<span data-ttu-id="48423-169">String</span><span class="sxs-lookup"><span data-stu-id="48423-169">String</span></span>|<span data-ttu-id="48423-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="48423-170">The more information Url.</span></span> <span data-ttu-id="48423-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-172">owner</span><span class="sxs-lookup"><span data-stu-id="48423-172">owner</span></span>|<span data-ttu-id="48423-173">String</span><span class="sxs-lookup"><span data-stu-id="48423-173">String</span></span>|<span data-ttu-id="48423-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-174">The owner of the app.</span></span> <span data-ttu-id="48423-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-176">developer</span><span class="sxs-lookup"><span data-stu-id="48423-176">developer</span></span>|<span data-ttu-id="48423-177">String</span><span class="sxs-lookup"><span data-stu-id="48423-177">String</span></span>|<span data-ttu-id="48423-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-178">The developer of the app.</span></span> <span data-ttu-id="48423-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-180">notes</span><span class="sxs-lookup"><span data-stu-id="48423-180">notes</span></span>|<span data-ttu-id="48423-181">String</span><span class="sxs-lookup"><span data-stu-id="48423-181">String</span></span>|<span data-ttu-id="48423-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="48423-182">Notes for the app.</span></span> <span data-ttu-id="48423-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="48423-184">uploadState</span></span>|<span data-ttu-id="48423-185">Int32</span><span class="sxs-lookup"><span data-stu-id="48423-185">Int32</span></span>|<span data-ttu-id="48423-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="48423-186">The upload state.</span></span> <span data-ttu-id="48423-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48423-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="48423-188">publishingState</span></span>|[<span data-ttu-id="48423-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48423-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48423-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-190">The publishing state for the app.</span></span> <span data-ttu-id="48423-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="48423-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48423-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="48423-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="48423-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48423-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="48423-194">committedContentVersion</span></span>|<span data-ttu-id="48423-195">String</span><span class="sxs-lookup"><span data-stu-id="48423-195">String</span></span>|<span data-ttu-id="48423-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="48423-196">The internal committed content version.</span></span> <span data-ttu-id="48423-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="48423-198">fileName</span><span class="sxs-lookup"><span data-stu-id="48423-198">fileName</span></span>|<span data-ttu-id="48423-199">String</span><span class="sxs-lookup"><span data-stu-id="48423-199">String</span></span>|<span data-ttu-id="48423-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-200">The name of the main Lob application file.</span></span> <span data-ttu-id="48423-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="48423-202">size</span><span class="sxs-lookup"><span data-stu-id="48423-202">size</span></span>|<span data-ttu-id="48423-203">Int64</span><span class="sxs-lookup"><span data-stu-id="48423-203">Int64</span></span>|<span data-ttu-id="48423-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="48423-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="48423-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="48423-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="48423-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="48423-206">commandLine</span></span>|<span data-ttu-id="48423-207">String</span><span class="sxs-lookup"><span data-stu-id="48423-207">String</span></span>|<span data-ttu-id="48423-208">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="48423-208">The command line.</span></span>|
|<span data-ttu-id="48423-209">productCode</span><span class="sxs-lookup"><span data-stu-id="48423-209">productCode</span></span>|<span data-ttu-id="48423-210">String</span><span class="sxs-lookup"><span data-stu-id="48423-210">String</span></span>|<span data-ttu-id="48423-211">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="48423-211">The product code.</span></span>|
|<span data-ttu-id="48423-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="48423-212">productVersion</span></span>|<span data-ttu-id="48423-213">String</span><span class="sxs-lookup"><span data-stu-id="48423-213">String</span></span>|<span data-ttu-id="48423-214">Версия бизнес-приложения MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="48423-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="48423-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="48423-215">ignoreVersionDetection</span></span>|<span data-ttu-id="48423-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="48423-216">Boolean</span></span>|<span data-ttu-id="48423-217">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="48423-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="48423-218">Для бизнес-приложений MSI Windows Mobile с функцией самостоятельного обновления следует использовать значение true.</span><span class="sxs-lookup"><span data-stu-id="48423-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="48423-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="48423-219">identityVersion</span></span>|<span data-ttu-id="48423-220">String</span><span class="sxs-lookup"><span data-stu-id="48423-220">String</span></span>|<span data-ttu-id="48423-221">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="48423-221">The identity version.</span></span>|
|<span data-ttu-id="48423-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="48423-222">useDeviceContext</span></span>|<span data-ttu-id="48423-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="48423-223">Boolean</span></span>|<span data-ttu-id="48423-224">Указывает, следует ли установить MSI двумя режимами в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="48423-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="48423-225">Если значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="48423-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="48423-226">Если задано значение false, приложение будет установлено для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="48423-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="48423-227">Если значение null, служба будет использовать пакет MSI контекст установки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="48423-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="48423-228">В случае MSI двумя режимами это значение по умолчанию будет пользователя.</span><span class="sxs-lookup"><span data-stu-id="48423-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="48423-229">Не могут задаваться для приложений двумя режимами.</span><span class="sxs-lookup"><span data-stu-id="48423-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="48423-230">Нельзя изменить после первоначального создания приложения.</span><span class="sxs-lookup"><span data-stu-id="48423-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="48423-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="48423-231">Response</span></span>
<span data-ttu-id="48423-232">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48423-232">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48423-233">Пример</span><span class="sxs-lookup"><span data-stu-id="48423-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="48423-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="48423-234">Request</span></span>
<span data-ttu-id="48423-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48423-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="48423-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="48423-236">Response</span></span>
<span data-ttu-id="48423-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48423-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





