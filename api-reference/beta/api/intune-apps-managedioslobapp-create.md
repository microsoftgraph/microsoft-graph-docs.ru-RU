---
title: Create managedIOSLobApp
description: Создание объекта managedIOSLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b2bbd4ff7721f4d89dc3b201a2c58277d9f0baca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936153"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="3b33f-103">Create managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="3b33f-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="3b33f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b33f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b33f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b33f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b33f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b33f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b33f-107">Создание объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b33f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3b33f-108">Prerequisites</span></span>
<span data-ttu-id="3b33f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b33f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b33f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b33f-111">Permission type</span></span>|<span data-ttu-id="3b33f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b33f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b33f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b33f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b33f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b33f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b33f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b33f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b33f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b33f-116">Not supported.</span></span>|
|<span data-ttu-id="3b33f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b33f-117">Application</span></span>|<span data-ttu-id="3b33f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b33f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b33f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b33f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3b33f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b33f-120">Request headers</span></span>
|<span data-ttu-id="3b33f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b33f-121">Header</span></span>|<span data-ttu-id="3b33f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b33f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b33f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b33f-123">Authorization</span></span>|<span data-ttu-id="3b33f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b33f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b33f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b33f-125">Accept</span></span>|<span data-ttu-id="3b33f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b33f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b33f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b33f-127">Request body</span></span>
<span data-ttu-id="3b33f-128">В тексте запроса добавьте представление объекта managedIOSLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b33f-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="3b33f-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="3b33f-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="3b33f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b33f-130">Property</span></span>|<span data-ttu-id="3b33f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b33f-131">Type</span></span>|<span data-ttu-id="3b33f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b33f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b33f-133">id</span><span class="sxs-lookup"><span data-stu-id="3b33f-133">id</span></span>|<span data-ttu-id="3b33f-134">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-134">String</span></span>|<span data-ttu-id="3b33f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b33f-135">Key of the entity.</span></span> <span data-ttu-id="3b33f-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3b33f-137">displayName</span></span>|<span data-ttu-id="3b33f-138">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-138">String</span></span>|<span data-ttu-id="3b33f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3b33f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3b33f-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-141">описание</span><span class="sxs-lookup"><span data-stu-id="3b33f-141">description</span></span>|<span data-ttu-id="3b33f-142">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-142">String</span></span>|<span data-ttu-id="3b33f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-143">The description of the app.</span></span> <span data-ttu-id="3b33f-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3b33f-145">publisher</span></span>|<span data-ttu-id="3b33f-146">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-146">String</span></span>|<span data-ttu-id="3b33f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-147">The publisher of the app.</span></span> <span data-ttu-id="3b33f-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3b33f-149">largeIcon</span></span>|[<span data-ttu-id="3b33f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b33f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b33f-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3b33f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3b33f-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b33f-153">createdDateTime</span></span>|<span data-ttu-id="3b33f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b33f-154">DateTimeOffset</span></span>|<span data-ttu-id="3b33f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-155">The date and time the app was created.</span></span> <span data-ttu-id="3b33f-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b33f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3b33f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b33f-158">DateTimeOffset</span></span>|<span data-ttu-id="3b33f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3b33f-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3b33f-161">isFeatured</span></span>|<span data-ttu-id="3b33f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b33f-162">Boolean</span></span>|<span data-ttu-id="3b33f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b33f-164">privacyInformationUrl</span></span>|<span data-ttu-id="3b33f-165">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-165">String</span></span>|<span data-ttu-id="3b33f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3b33f-166">The privacy statement Url.</span></span> <span data-ttu-id="3b33f-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b33f-168">informationUrl</span></span>|<span data-ttu-id="3b33f-169">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-169">String</span></span>|<span data-ttu-id="3b33f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3b33f-170">The more information Url.</span></span> <span data-ttu-id="3b33f-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-172">owner</span><span class="sxs-lookup"><span data-stu-id="3b33f-172">owner</span></span>|<span data-ttu-id="3b33f-173">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-173">String</span></span>|<span data-ttu-id="3b33f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-174">The owner of the app.</span></span> <span data-ttu-id="3b33f-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-176">developer</span><span class="sxs-lookup"><span data-stu-id="3b33f-176">developer</span></span>|<span data-ttu-id="3b33f-177">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-177">String</span></span>|<span data-ttu-id="3b33f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-178">The developer of the app.</span></span> <span data-ttu-id="3b33f-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-180">notes</span><span class="sxs-lookup"><span data-stu-id="3b33f-180">notes</span></span>|<span data-ttu-id="3b33f-181">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-181">String</span></span>|<span data-ttu-id="3b33f-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="3b33f-182">Notes for the app.</span></span> <span data-ttu-id="3b33f-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3b33f-184">uploadState</span></span>|<span data-ttu-id="3b33f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3b33f-185">Int32</span></span>|<span data-ttu-id="3b33f-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="3b33f-186">The upload state.</span></span> <span data-ttu-id="3b33f-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b33f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3b33f-188">publishingState</span></span>|[<span data-ttu-id="3b33f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3b33f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3b33f-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-190">The publishing state for the app.</span></span> <span data-ttu-id="3b33f-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3b33f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3b33f-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3b33f-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3b33f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3b33f-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3b33f-194">appAvailability</span></span>|[<span data-ttu-id="3b33f-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="3b33f-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="3b33f-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-196">The Application's availability.</span></span> <span data-ttu-id="3b33f-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="3b33f-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="3b33f-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="3b33f-199">version</span><span class="sxs-lookup"><span data-stu-id="3b33f-199">version</span></span>|<span data-ttu-id="3b33f-200">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-200">String</span></span>|<span data-ttu-id="3b33f-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-201">The Application's version.</span></span> <span data-ttu-id="3b33f-202">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="3b33f-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3b33f-203">committedContentVersion</span></span>|<span data-ttu-id="3b33f-204">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-204">String</span></span>|<span data-ttu-id="3b33f-205">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="3b33f-205">The internal committed content version.</span></span> <span data-ttu-id="3b33f-206">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b33f-207">fileName</span><span class="sxs-lookup"><span data-stu-id="3b33f-207">fileName</span></span>|<span data-ttu-id="3b33f-208">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-208">String</span></span>|<span data-ttu-id="3b33f-209">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-209">The name of the main Lob application file.</span></span> <span data-ttu-id="3b33f-210">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b33f-211">size</span><span class="sxs-lookup"><span data-stu-id="3b33f-211">size</span></span>|<span data-ttu-id="3b33f-212">Int64</span><span class="sxs-lookup"><span data-stu-id="3b33f-212">Int64</span></span>|<span data-ttu-id="3b33f-213">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="3b33f-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="3b33f-214">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b33f-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b33f-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="3b33f-215">bundleId</span></span>|<span data-ttu-id="3b33f-216">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-216">String</span></span>|<span data-ttu-id="3b33f-217">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-217">The Identity Name.</span></span>|
|<span data-ttu-id="3b33f-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3b33f-218">applicableDeviceType</span></span>|[<span data-ttu-id="3b33f-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3b33f-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3b33f-220">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="3b33f-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3b33f-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b33f-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3b33f-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b33f-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3b33f-223">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3b33f-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3b33f-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b33f-224">expirationDateTime</span></span>|<span data-ttu-id="3b33f-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b33f-225">DateTimeOffset</span></span>|<span data-ttu-id="3b33f-226">Время окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="3b33f-226">The expiration time.</span></span>|
|<span data-ttu-id="3b33f-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3b33f-227">versionNumber</span></span>|<span data-ttu-id="3b33f-228">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-228">String</span></span>|<span data-ttu-id="3b33f-229">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="3b33f-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3b33f-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3b33f-230">buildNumber</span></span>|<span data-ttu-id="3b33f-231">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-231">String</span></span>|<span data-ttu-id="3b33f-232">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="3b33f-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3b33f-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3b33f-233">identityVersion</span></span>|<span data-ttu-id="3b33f-234">String</span><span class="sxs-lookup"><span data-stu-id="3b33f-234">String</span></span>|<span data-ttu-id="3b33f-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3b33f-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3b33f-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b33f-236">Response</span></span>
<span data-ttu-id="3b33f-237">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3b33f-237">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b33f-238">Пример</span><span class="sxs-lookup"><span data-stu-id="3b33f-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b33f-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b33f-239">Request</span></span>
<span data-ttu-id="3b33f-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b33f-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1421

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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

### <a name="response"></a><span data-ttu-id="3b33f-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b33f-241">Response</span></span>
<span data-ttu-id="3b33f-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3b33f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





