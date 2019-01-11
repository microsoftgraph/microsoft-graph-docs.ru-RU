---
title: Обновление macOSLobApp
description: Обновление свойства объекта macOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 35889053c1bdebcddea9ffd5f69a754530d7ebc5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859418"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="9aed0-103">Обновление macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="9aed0-103">Update macOSLobApp</span></span>

> <span data-ttu-id="9aed0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9aed0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aed0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aed0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9aed0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9aed0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9aed0-107">Обновление свойства объекта [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9aed0-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9aed0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9aed0-108">Prerequisites</span></span>
<span data-ttu-id="9aed0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9aed0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9aed0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9aed0-111">Permission type</span></span>|<span data-ttu-id="9aed0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9aed0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9aed0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9aed0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9aed0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9aed0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9aed0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9aed0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9aed0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aed0-116">Not supported.</span></span>|
|<span data-ttu-id="9aed0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9aed0-117">Application</span></span>|<span data-ttu-id="9aed0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aed0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9aed0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9aed0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9aed0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9aed0-120">Request headers</span></span>
|<span data-ttu-id="9aed0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9aed0-121">Header</span></span>|<span data-ttu-id="9aed0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9aed0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9aed0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9aed0-123">Authorization</span></span>|<span data-ttu-id="9aed0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9aed0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9aed0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9aed0-125">Accept</span></span>|<span data-ttu-id="9aed0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9aed0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9aed0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9aed0-127">Request body</span></span>
<span data-ttu-id="9aed0-128">В тексте запроса укажите представление JSON для объекта [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9aed0-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="9aed0-129">В следующей таблице показаны свойства, которые необходимы для создания [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="9aed0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9aed0-130">Property</span></span>|<span data-ttu-id="9aed0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9aed0-131">Type</span></span>|<span data-ttu-id="9aed0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9aed0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aed0-133">id</span><span class="sxs-lookup"><span data-stu-id="9aed0-133">id</span></span>|<span data-ttu-id="9aed0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9aed0-134">String</span></span>|<span data-ttu-id="9aed0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9aed0-135">Key of the entity.</span></span> <span data-ttu-id="9aed0-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9aed0-137">displayName</span></span>|<span data-ttu-id="9aed0-138">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-138">String</span></span>|<span data-ttu-id="9aed0-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9aed0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9aed0-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-141">описание</span><span class="sxs-lookup"><span data-stu-id="9aed0-141">description</span></span>|<span data-ttu-id="9aed0-142">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-142">String</span></span>|<span data-ttu-id="9aed0-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-143">The description of the app.</span></span> <span data-ttu-id="9aed0-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9aed0-145">publisher</span></span>|<span data-ttu-id="9aed0-146">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-146">String</span></span>|<span data-ttu-id="9aed0-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-147">The publisher of the app.</span></span> <span data-ttu-id="9aed0-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9aed0-149">largeIcon</span></span>|[<span data-ttu-id="9aed0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9aed0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9aed0-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9aed0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9aed0-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9aed0-153">createdDateTime</span></span>|<span data-ttu-id="9aed0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aed0-154">DateTimeOffset</span></span>|<span data-ttu-id="9aed0-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-155">The date and time the app was created.</span></span> <span data-ttu-id="9aed0-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9aed0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9aed0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aed0-158">DateTimeOffset</span></span>|<span data-ttu-id="9aed0-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9aed0-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9aed0-161">isFeatured</span></span>|<span data-ttu-id="9aed0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9aed0-162">Boolean</span></span>|<span data-ttu-id="9aed0-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9aed0-164">privacyInformationUrl</span></span>|<span data-ttu-id="9aed0-165">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-165">String</span></span>|<span data-ttu-id="9aed0-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9aed0-166">The privacy statement Url.</span></span> <span data-ttu-id="9aed0-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9aed0-168">informationUrl</span></span>|<span data-ttu-id="9aed0-169">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-169">String</span></span>|<span data-ttu-id="9aed0-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9aed0-170">The more information Url.</span></span> <span data-ttu-id="9aed0-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-172">owner</span><span class="sxs-lookup"><span data-stu-id="9aed0-172">owner</span></span>|<span data-ttu-id="9aed0-173">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-173">String</span></span>|<span data-ttu-id="9aed0-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-174">The owner of the app.</span></span> <span data-ttu-id="9aed0-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-176">developer</span><span class="sxs-lookup"><span data-stu-id="9aed0-176">developer</span></span>|<span data-ttu-id="9aed0-177">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-177">String</span></span>|<span data-ttu-id="9aed0-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-178">The developer of the app.</span></span> <span data-ttu-id="9aed0-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-180">notes</span><span class="sxs-lookup"><span data-stu-id="9aed0-180">notes</span></span>|<span data-ttu-id="9aed0-181">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-181">String</span></span>|<span data-ttu-id="9aed0-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="9aed0-182">Notes for the app.</span></span> <span data-ttu-id="9aed0-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9aed0-184">uploadState</span></span>|<span data-ttu-id="9aed0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9aed0-185">Int32</span></span>|<span data-ttu-id="9aed0-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="9aed0-186">The upload state.</span></span> <span data-ttu-id="9aed0-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9aed0-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9aed0-188">publishingState</span></span>|[<span data-ttu-id="9aed0-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9aed0-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9aed0-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-190">The publishing state for the app.</span></span> <span data-ttu-id="9aed0-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9aed0-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9aed0-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9aed0-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9aed0-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9aed0-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9aed0-194">committedContentVersion</span></span>|<span data-ttu-id="9aed0-195">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-195">String</span></span>|<span data-ttu-id="9aed0-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="9aed0-196">The internal committed content version.</span></span> <span data-ttu-id="9aed0-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9aed0-198">fileName</span><span class="sxs-lookup"><span data-stu-id="9aed0-198">fileName</span></span>|<span data-ttu-id="9aed0-199">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-199">String</span></span>|<span data-ttu-id="9aed0-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-200">The name of the main Lob application file.</span></span> <span data-ttu-id="9aed0-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9aed0-202">size</span><span class="sxs-lookup"><span data-stu-id="9aed0-202">size</span></span>|<span data-ttu-id="9aed0-203">Int64</span><span class="sxs-lookup"><span data-stu-id="9aed0-203">Int64</span></span>|<span data-ttu-id="9aed0-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="9aed0-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="9aed0-205">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9aed0-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9aed0-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="9aed0-206">bundleId</span></span>|<span data-ttu-id="9aed0-207">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-207">String</span></span>|<span data-ttu-id="9aed0-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="9aed0-208">The bundle id.</span></span>|
|<span data-ttu-id="9aed0-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9aed0-209">minimumSupportedOperatingSystem</span></span>|<span data-ttu-id="9aed0-210">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md);</span><span class="sxs-lookup"><span data-stu-id="9aed0-210">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)</span></span>|<span data-ttu-id="9aed0-211">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9aed0-211">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9aed0-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9aed0-212">buildNumber</span></span>|<span data-ttu-id="9aed0-213">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-213">String</span></span>|<span data-ttu-id="9aed0-214">Номер построения строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-214">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9aed0-215">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9aed0-215">versionNumber</span></span>|<span data-ttu-id="9aed0-216">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-216">String</span></span>|<span data-ttu-id="9aed0-217">Номер версии строки MacOS бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-217">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9aed0-218">childApps</span><span class="sxs-lookup"><span data-stu-id="9aed0-218">childApps</span></span>|<span data-ttu-id="9aed0-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9aed0-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="9aed0-220">Список приложения в этот пакет пакета</span><span class="sxs-lookup"><span data-stu-id="9aed0-220">The app list in this bundle package</span></span>|
|<span data-ttu-id="9aed0-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9aed0-221">identityVersion</span></span>|<span data-ttu-id="9aed0-222">String</span><span class="sxs-lookup"><span data-stu-id="9aed0-222">String</span></span>|<span data-ttu-id="9aed0-223">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9aed0-223">The identity version.</span></span>|
|<span data-ttu-id="9aed0-224">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="9aed0-224">md5HashChunkSize</span></span>|<span data-ttu-id="9aed0-225">Int32</span><span class="sxs-lookup"><span data-stu-id="9aed0-225">Int32</span></span>|<span data-ttu-id="9aed0-226">Размер блока для хеша MD5</span><span class="sxs-lookup"><span data-stu-id="9aed0-226">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="9aed0-227">md5Hash</span><span class="sxs-lookup"><span data-stu-id="9aed0-227">md5Hash</span></span>|<span data-ttu-id="9aed0-228">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9aed0-228">String collection</span></span>|<span data-ttu-id="9aed0-229">MD5 хэш-кодов</span><span class="sxs-lookup"><span data-stu-id="9aed0-229">The MD5 hash codes</span></span>|
|<span data-ttu-id="9aed0-230">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="9aed0-230">ignoreVersionDetection</span></span>|<span data-ttu-id="9aed0-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9aed0-231">Boolean</span></span>|<span data-ttu-id="9aed0-232">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9aed0-232">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="9aed0-233">Задайте значение true для macOS строки из бизнес-приложений, использующих функции самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="9aed0-233">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="9aed0-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="9aed0-234">Response</span></span>
<span data-ttu-id="9aed0-235">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOSLobApp](../resources/intune-apps-macoslobapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9aed0-235">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9aed0-236">Пример</span><span class="sxs-lookup"><span data-stu-id="9aed0-236">Example</span></span>
### <a name="request"></a><span data-ttu-id="9aed0-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="9aed0-237">Request</span></span>
<span data-ttu-id="9aed0-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9aed0-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1476

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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="9aed0-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="9aed0-239">Response</span></span>
<span data-ttu-id="9aed0-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9aed0-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```





