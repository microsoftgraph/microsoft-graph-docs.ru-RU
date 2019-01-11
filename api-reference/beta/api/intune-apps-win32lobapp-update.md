---
title: Обновление win32LobApp
description: Обновление свойства объекта win32LobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2deac829d1aad6cf0b1a1f3ec4a2a91e7b07c6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864934"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="46f4a-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="46f4a-103">Update win32LobApp</span></span>

> <span data-ttu-id="46f4a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46f4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46f4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46f4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46f4a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="46f4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46f4a-107">Обновление свойства объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="46f4a-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="46f4a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46f4a-108">Prerequisites</span></span>
<span data-ttu-id="46f4a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46f4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46f4a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46f4a-111">Permission type</span></span>|<span data-ttu-id="46f4a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46f4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46f4a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46f4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46f4a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46f4a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46f4a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46f4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46f4a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46f4a-116">Not supported.</span></span>|
|<span data-ttu-id="46f4a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46f4a-117">Application</span></span>|<span data-ttu-id="46f4a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46f4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46f4a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46f4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="46f4a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46f4a-120">Request headers</span></span>
|<span data-ttu-id="46f4a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46f4a-121">Header</span></span>|<span data-ttu-id="46f4a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46f4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46f4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46f4a-123">Authorization</span></span>|<span data-ttu-id="46f4a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46f4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46f4a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46f4a-125">Accept</span></span>|<span data-ttu-id="46f4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46f4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46f4a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46f4a-127">Request body</span></span>
<span data-ttu-id="46f4a-128">В тексте запроса укажите представление JSON для объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="46f4a-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="46f4a-129">В следующей таблице показаны свойства, которые необходимы для создания [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="46f4a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="46f4a-130">Property</span></span>|<span data-ttu-id="46f4a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46f4a-131">Type</span></span>|<span data-ttu-id="46f4a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46f4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46f4a-133">id</span><span class="sxs-lookup"><span data-stu-id="46f4a-133">id</span></span>|<span data-ttu-id="46f4a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="46f4a-134">String</span></span>|<span data-ttu-id="46f4a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46f4a-135">Key of the entity.</span></span> <span data-ttu-id="46f4a-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="46f4a-137">displayName</span></span>|<span data-ttu-id="46f4a-138">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-138">String</span></span>|<span data-ttu-id="46f4a-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="46f4a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="46f4a-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-141">описание</span><span class="sxs-lookup"><span data-stu-id="46f4a-141">description</span></span>|<span data-ttu-id="46f4a-142">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-142">String</span></span>|<span data-ttu-id="46f4a-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-143">The description of the app.</span></span> <span data-ttu-id="46f4a-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="46f4a-145">publisher</span></span>|<span data-ttu-id="46f4a-146">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-146">String</span></span>|<span data-ttu-id="46f4a-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-147">The publisher of the app.</span></span> <span data-ttu-id="46f4a-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="46f4a-149">largeIcon</span></span>|[<span data-ttu-id="46f4a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="46f4a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="46f4a-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="46f4a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="46f4a-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46f4a-153">createdDateTime</span></span>|<span data-ttu-id="46f4a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46f4a-154">DateTimeOffset</span></span>|<span data-ttu-id="46f4a-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-155">The date and time the app was created.</span></span> <span data-ttu-id="46f4a-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46f4a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="46f4a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46f4a-158">DateTimeOffset</span></span>|<span data-ttu-id="46f4a-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="46f4a-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="46f4a-161">isFeatured</span></span>|<span data-ttu-id="46f4a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="46f4a-162">Boolean</span></span>|<span data-ttu-id="46f4a-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="46f4a-164">privacyInformationUrl</span></span>|<span data-ttu-id="46f4a-165">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-165">String</span></span>|<span data-ttu-id="46f4a-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="46f4a-166">The privacy statement Url.</span></span> <span data-ttu-id="46f4a-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="46f4a-168">informationUrl</span></span>|<span data-ttu-id="46f4a-169">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-169">String</span></span>|<span data-ttu-id="46f4a-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="46f4a-170">The more information Url.</span></span> <span data-ttu-id="46f4a-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-172">owner</span><span class="sxs-lookup"><span data-stu-id="46f4a-172">owner</span></span>|<span data-ttu-id="46f4a-173">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-173">String</span></span>|<span data-ttu-id="46f4a-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-174">The owner of the app.</span></span> <span data-ttu-id="46f4a-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-176">developer</span><span class="sxs-lookup"><span data-stu-id="46f4a-176">developer</span></span>|<span data-ttu-id="46f4a-177">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-177">String</span></span>|<span data-ttu-id="46f4a-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-178">The developer of the app.</span></span> <span data-ttu-id="46f4a-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-180">notes</span><span class="sxs-lookup"><span data-stu-id="46f4a-180">notes</span></span>|<span data-ttu-id="46f4a-181">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-181">String</span></span>|<span data-ttu-id="46f4a-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="46f4a-182">Notes for the app.</span></span> <span data-ttu-id="46f4a-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="46f4a-184">uploadState</span></span>|<span data-ttu-id="46f4a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="46f4a-185">Int32</span></span>|<span data-ttu-id="46f4a-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="46f4a-186">The upload state.</span></span> <span data-ttu-id="46f4a-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="46f4a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="46f4a-188">publishingState</span></span>|[<span data-ttu-id="46f4a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="46f4a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="46f4a-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-190">The publishing state for the app.</span></span> <span data-ttu-id="46f4a-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="46f4a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="46f4a-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="46f4a-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="46f4a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="46f4a-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="46f4a-194">committedContentVersion</span></span>|<span data-ttu-id="46f4a-195">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-195">String</span></span>|<span data-ttu-id="46f4a-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="46f4a-196">The internal committed content version.</span></span> <span data-ttu-id="46f4a-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="46f4a-198">fileName</span><span class="sxs-lookup"><span data-stu-id="46f4a-198">fileName</span></span>|<span data-ttu-id="46f4a-199">String</span><span class="sxs-lookup"><span data-stu-id="46f4a-199">String</span></span>|<span data-ttu-id="46f4a-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-200">The name of the main Lob application file.</span></span> <span data-ttu-id="46f4a-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="46f4a-202">size</span><span class="sxs-lookup"><span data-stu-id="46f4a-202">size</span></span>|<span data-ttu-id="46f4a-203">Int64</span><span class="sxs-lookup"><span data-stu-id="46f4a-203">Int64</span></span>|<span data-ttu-id="46f4a-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="46f4a-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="46f4a-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="46f4a-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="46f4a-206">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="46f4a-206">installCommandLine</span></span>|<span data-ttu-id="46f4a-207">Строка</span><span class="sxs-lookup"><span data-stu-id="46f4a-207">String</span></span>|<span data-ttu-id="46f4a-208">Командной строки для установки этого приложения</span><span class="sxs-lookup"><span data-stu-id="46f4a-208">The command line to install this app</span></span>|
|<span data-ttu-id="46f4a-209">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="46f4a-209">uninstallCommandLine</span></span>|<span data-ttu-id="46f4a-210">Строка</span><span class="sxs-lookup"><span data-stu-id="46f4a-210">String</span></span>|<span data-ttu-id="46f4a-211">В командной строке команду Удалить это приложение</span><span class="sxs-lookup"><span data-stu-id="46f4a-211">The command line to uninstall this app</span></span>|
|<span data-ttu-id="46f4a-212">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="46f4a-212">applicableArchitectures</span></span>|[<span data-ttu-id="46f4a-213">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="46f4a-213">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="46f4a-214">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="46f4a-214">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="46f4a-215">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="46f4a-215">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="46f4a-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="46f4a-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="46f4a-217">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="46f4a-217">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="46f4a-218">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="46f4a-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="46f4a-219">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="46f4a-219">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="46f4a-220">Int32</span><span class="sxs-lookup"><span data-stu-id="46f4a-220">Int32</span></span>|<span data-ttu-id="46f4a-221">Значение для минимального свободного дискового пространства, которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-221">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="46f4a-222">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="46f4a-222">minimumMemoryInMB</span></span>|<span data-ttu-id="46f4a-223">Int32</span><span class="sxs-lookup"><span data-stu-id="46f4a-223">Int32</span></span>|<span data-ttu-id="46f4a-224">Значение для минимального физической памяти, которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-224">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="46f4a-225">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="46f4a-225">minimumNumberOfProcessors</span></span>|<span data-ttu-id="46f4a-226">Int32</span><span class="sxs-lookup"><span data-stu-id="46f4a-226">Int32</span></span>|<span data-ttu-id="46f4a-227">Значение для минимальное число процессоров которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-227">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="46f4a-228">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="46f4a-228">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="46f4a-229">Int32</span><span class="sxs-lookup"><span data-stu-id="46f4a-229">Int32</span></span>|<span data-ttu-id="46f4a-230">Значение для минимальная скорость ЦП, которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-230">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="46f4a-231">detectionRules</span><span class="sxs-lookup"><span data-stu-id="46f4a-231">detectionRules</span></span>|<span data-ttu-id="46f4a-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="46f4a-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="46f4a-233">Определение правил для обнаружения Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-233">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="46f4a-234">installExperience</span><span class="sxs-lookup"><span data-stu-id="46f4a-234">installExperience</span></span>|[<span data-ttu-id="46f4a-235">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="46f4a-235">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="46f4a-236">Опыт установки для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="46f4a-236">The install experience for this app.</span></span>|
|<span data-ttu-id="46f4a-237">returnCodes</span><span class="sxs-lookup"><span data-stu-id="46f4a-237">returnCodes</span></span>|<span data-ttu-id="46f4a-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="46f4a-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="46f4a-239">Коды возврата для записи поведение при установке.</span><span class="sxs-lookup"><span data-stu-id="46f4a-239">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="46f4a-240">msiInformation</span><span class="sxs-lookup"><span data-stu-id="46f4a-240">msiInformation</span></span>|[<span data-ttu-id="46f4a-241">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="46f4a-241">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="46f4a-242">Подробности MSI, если это приложение Win32 представляет собой приложение MSI.</span><span class="sxs-lookup"><span data-stu-id="46f4a-242">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="46f4a-243">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="46f4a-243">setupFilePath</span></span>|<span data-ttu-id="46f4a-244">Строка</span><span class="sxs-lookup"><span data-stu-id="46f4a-244">String</span></span>|<span data-ttu-id="46f4a-245">Относительный путь к файлу программы установки в пакете зашифрованные Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="46f4a-245">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="46f4a-246">Ответ</span><span class="sxs-lookup"><span data-stu-id="46f4a-246">Response</span></span>
<span data-ttu-id="46f4a-247">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [win32LobApp](../resources/intune-apps-win32lobapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="46f4a-247">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46f4a-248">Пример</span><span class="sxs-lookup"><span data-stu-id="46f4a-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="46f4a-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="46f4a-249">Request</span></span>
<span data-ttu-id="46f4a-250">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46f4a-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2214

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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="46f4a-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="46f4a-251">Response</span></span>
<span data-ttu-id="46f4a-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46f4a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2372

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```





