---
title: Create androidLobApp
description: Создание нового объекта androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 86cd6e0d62ebf226f82d94a6a023701bdd82e405
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966806"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="b9e70-103">Create androidLobApp</span><span class="sxs-lookup"><span data-stu-id="b9e70-103">Create androidLobApp</span></span>

> <span data-ttu-id="b9e70-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9e70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9e70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9e70-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9e70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9e70-107">Создание нового объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9e70-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b9e70-108">Prerequisites</span></span>
<span data-ttu-id="b9e70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9e70-111">Permission type</span></span>|<span data-ttu-id="b9e70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9e70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9e70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9e70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9e70-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e70-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9e70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9e70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9e70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e70-116">Not supported.</span></span>|
|<span data-ttu-id="b9e70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9e70-117">Application</span></span>|<span data-ttu-id="b9e70-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e70-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9e70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9e70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b9e70-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9e70-120">Request headers</span></span>
|<span data-ttu-id="b9e70-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9e70-121">Header</span></span>|<span data-ttu-id="b9e70-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9e70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9e70-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9e70-123">Authorization</span></span>|<span data-ttu-id="b9e70-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b9e70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9e70-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9e70-125">Accept</span></span>|<span data-ttu-id="b9e70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9e70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e70-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9e70-127">Request body</span></span>
<span data-ttu-id="b9e70-128">В теле запроса добавьте представление объекта androidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9e70-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="b9e70-129">Ниже показаны свойства, которые необходимо указывать при создании объекта androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="b9e70-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="b9e70-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9e70-130">Property</span></span>|<span data-ttu-id="b9e70-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9e70-131">Type</span></span>|<span data-ttu-id="b9e70-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9e70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e70-133">id</span><span class="sxs-lookup"><span data-stu-id="b9e70-133">id</span></span>|<span data-ttu-id="b9e70-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b9e70-134">String</span></span>|<span data-ttu-id="b9e70-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9e70-135">Key of the entity.</span></span> <span data-ttu-id="b9e70-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b9e70-137">displayName</span></span>|<span data-ttu-id="b9e70-138">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-138">String</span></span>|<span data-ttu-id="b9e70-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b9e70-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b9e70-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-141">описание</span><span class="sxs-lookup"><span data-stu-id="b9e70-141">description</span></span>|<span data-ttu-id="b9e70-142">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-142">String</span></span>|<span data-ttu-id="b9e70-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-143">The description of the app.</span></span> <span data-ttu-id="b9e70-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b9e70-145">publisher</span></span>|<span data-ttu-id="b9e70-146">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-146">String</span></span>|<span data-ttu-id="b9e70-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-147">The publisher of the app.</span></span> <span data-ttu-id="b9e70-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b9e70-149">largeIcon</span></span>|[<span data-ttu-id="b9e70-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b9e70-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b9e70-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b9e70-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b9e70-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9e70-153">createdDateTime</span></span>|<span data-ttu-id="b9e70-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9e70-154">DateTimeOffset</span></span>|<span data-ttu-id="b9e70-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-155">The date and time the app was created.</span></span> <span data-ttu-id="b9e70-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9e70-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b9e70-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9e70-158">DateTimeOffset</span></span>|<span data-ttu-id="b9e70-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b9e70-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b9e70-161">isFeatured</span></span>|<span data-ttu-id="b9e70-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9e70-162">Boolean</span></span>|<span data-ttu-id="b9e70-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b9e70-164">privacyInformationUrl</span></span>|<span data-ttu-id="b9e70-165">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-165">String</span></span>|<span data-ttu-id="b9e70-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b9e70-166">The privacy statement Url.</span></span> <span data-ttu-id="b9e70-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b9e70-168">informationUrl</span></span>|<span data-ttu-id="b9e70-169">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-169">String</span></span>|<span data-ttu-id="b9e70-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b9e70-170">The more information Url.</span></span> <span data-ttu-id="b9e70-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-172">owner</span><span class="sxs-lookup"><span data-stu-id="b9e70-172">owner</span></span>|<span data-ttu-id="b9e70-173">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-173">String</span></span>|<span data-ttu-id="b9e70-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-174">The owner of the app.</span></span> <span data-ttu-id="b9e70-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-176">developer</span><span class="sxs-lookup"><span data-stu-id="b9e70-176">developer</span></span>|<span data-ttu-id="b9e70-177">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-177">String</span></span>|<span data-ttu-id="b9e70-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-178">The developer of the app.</span></span> <span data-ttu-id="b9e70-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-180">notes</span><span class="sxs-lookup"><span data-stu-id="b9e70-180">notes</span></span>|<span data-ttu-id="b9e70-181">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-181">String</span></span>|<span data-ttu-id="b9e70-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="b9e70-182">Notes for the app.</span></span> <span data-ttu-id="b9e70-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b9e70-184">uploadState</span></span>|<span data-ttu-id="b9e70-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b9e70-185">Int32</span></span>|<span data-ttu-id="b9e70-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="b9e70-186">The upload state.</span></span> <span data-ttu-id="b9e70-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b9e70-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b9e70-188">publishingState</span></span>|[<span data-ttu-id="b9e70-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b9e70-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b9e70-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-190">The publishing state for the app.</span></span> <span data-ttu-id="b9e70-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b9e70-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b9e70-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b9e70-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b9e70-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b9e70-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b9e70-194">committedContentVersion</span></span>|<span data-ttu-id="b9e70-195">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-195">String</span></span>|<span data-ttu-id="b9e70-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="b9e70-196">The internal committed content version.</span></span> <span data-ttu-id="b9e70-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b9e70-198">fileName</span><span class="sxs-lookup"><span data-stu-id="b9e70-198">fileName</span></span>|<span data-ttu-id="b9e70-199">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-199">String</span></span>|<span data-ttu-id="b9e70-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-200">The name of the main Lob application file.</span></span> <span data-ttu-id="b9e70-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b9e70-202">size</span><span class="sxs-lookup"><span data-stu-id="b9e70-202">size</span></span>|<span data-ttu-id="b9e70-203">Int64</span><span class="sxs-lookup"><span data-stu-id="b9e70-203">Int64</span></span>|<span data-ttu-id="b9e70-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="b9e70-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="b9e70-205">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b9e70-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b9e70-206">packageId</span><span class="sxs-lookup"><span data-stu-id="b9e70-206">packageId</span></span>|<span data-ttu-id="b9e70-207">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-207">String</span></span>|<span data-ttu-id="b9e70-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="b9e70-208">The package identifier.</span></span>|
|<span data-ttu-id="b9e70-209">identityName</span><span class="sxs-lookup"><span data-stu-id="b9e70-209">identityName</span></span>|<span data-ttu-id="b9e70-210">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-210">String</span></span>|<span data-ttu-id="b9e70-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-211">The Identity Name.</span></span>|
|<span data-ttu-id="b9e70-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b9e70-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b9e70-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b9e70-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b9e70-214">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b9e70-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b9e70-215">versionName</span><span class="sxs-lookup"><span data-stu-id="b9e70-215">versionName</span></span>|<span data-ttu-id="b9e70-216">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-216">String</span></span>|<span data-ttu-id="b9e70-217">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="b9e70-217">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b9e70-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="b9e70-218">versionCode</span></span>|<span data-ttu-id="b9e70-219">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-219">String</span></span>|<span data-ttu-id="b9e70-220">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="b9e70-220">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b9e70-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b9e70-221">identityVersion</span></span>|<span data-ttu-id="b9e70-222">String</span><span class="sxs-lookup"><span data-stu-id="b9e70-222">String</span></span>|<span data-ttu-id="b9e70-223">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b9e70-223">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="b9e70-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9e70-224">Response</span></span>
<span data-ttu-id="b9e70-225">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9e70-225">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e70-226">Пример</span><span class="sxs-lookup"><span data-stu-id="b9e70-226">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9e70-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9e70-227">Request</span></span>
<span data-ttu-id="b9e70-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9e70-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1365

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="b9e70-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9e70-229">Response</span></span>
<span data-ttu-id="b9e70-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9e70-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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





