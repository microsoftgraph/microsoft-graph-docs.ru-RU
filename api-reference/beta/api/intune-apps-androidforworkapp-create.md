---
title: Создание androidForWorkApp
description: Создание нового объекта androidForWorkApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4f557c9577d2b85e96038cc9976f9d19ddfaf867
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951910"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="013c3-103">Создание androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="013c3-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="013c3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="013c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="013c3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="013c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="013c3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="013c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="013c3-107">Создание нового объекта [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="013c3-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="013c3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="013c3-108">Prerequisites</span></span>
<span data-ttu-id="013c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="013c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="013c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="013c3-111">Permission type</span></span>|<span data-ttu-id="013c3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="013c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="013c3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="013c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="013c3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013c3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="013c3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="013c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="013c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="013c3-116">Not supported.</span></span>|
|<span data-ttu-id="013c3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="013c3-117">Application</span></span>|<span data-ttu-id="013c3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="013c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="013c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="013c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="013c3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="013c3-120">Request headers</span></span>
|<span data-ttu-id="013c3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="013c3-121">Header</span></span>|<span data-ttu-id="013c3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="013c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="013c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="013c3-123">Authorization</span></span>|<span data-ttu-id="013c3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="013c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="013c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="013c3-125">Accept</span></span>|<span data-ttu-id="013c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="013c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="013c3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="013c3-127">Request body</span></span>
<span data-ttu-id="013c3-128">В тексте запроса укажите представление JSON для объекта androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="013c3-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="013c3-129">В следующей таблице показаны свойства, которые необходимы для создания androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="013c3-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="013c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="013c3-130">Property</span></span>|<span data-ttu-id="013c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="013c3-131">Type</span></span>|<span data-ttu-id="013c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="013c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013c3-133">id</span><span class="sxs-lookup"><span data-stu-id="013c3-133">id</span></span>|<span data-ttu-id="013c3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="013c3-134">String</span></span>|<span data-ttu-id="013c3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="013c3-135">Key of the entity.</span></span> <span data-ttu-id="013c3-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="013c3-137">displayName</span></span>|<span data-ttu-id="013c3-138">String</span><span class="sxs-lookup"><span data-stu-id="013c3-138">String</span></span>|<span data-ttu-id="013c3-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="013c3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="013c3-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-141">описание</span><span class="sxs-lookup"><span data-stu-id="013c3-141">description</span></span>|<span data-ttu-id="013c3-142">String</span><span class="sxs-lookup"><span data-stu-id="013c3-142">String</span></span>|<span data-ttu-id="013c3-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-143">The description of the app.</span></span> <span data-ttu-id="013c3-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="013c3-145">publisher</span></span>|<span data-ttu-id="013c3-146">String</span><span class="sxs-lookup"><span data-stu-id="013c3-146">String</span></span>|<span data-ttu-id="013c3-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-147">The publisher of the app.</span></span> <span data-ttu-id="013c3-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="013c3-149">largeIcon</span></span>|[<span data-ttu-id="013c3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="013c3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="013c3-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="013c3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="013c3-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="013c3-153">createdDateTime</span></span>|<span data-ttu-id="013c3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="013c3-154">DateTimeOffset</span></span>|<span data-ttu-id="013c3-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-155">The date and time the app was created.</span></span> <span data-ttu-id="013c3-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="013c3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="013c3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="013c3-158">DateTimeOffset</span></span>|<span data-ttu-id="013c3-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="013c3-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="013c3-161">isFeatured</span></span>|<span data-ttu-id="013c3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="013c3-162">Boolean</span></span>|<span data-ttu-id="013c3-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="013c3-164">privacyInformationUrl</span></span>|<span data-ttu-id="013c3-165">String</span><span class="sxs-lookup"><span data-stu-id="013c3-165">String</span></span>|<span data-ttu-id="013c3-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="013c3-166">The privacy statement Url.</span></span> <span data-ttu-id="013c3-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="013c3-168">informationUrl</span></span>|<span data-ttu-id="013c3-169">String</span><span class="sxs-lookup"><span data-stu-id="013c3-169">String</span></span>|<span data-ttu-id="013c3-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="013c3-170">The more information Url.</span></span> <span data-ttu-id="013c3-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-172">owner</span><span class="sxs-lookup"><span data-stu-id="013c3-172">owner</span></span>|<span data-ttu-id="013c3-173">String</span><span class="sxs-lookup"><span data-stu-id="013c3-173">String</span></span>|<span data-ttu-id="013c3-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-174">The owner of the app.</span></span> <span data-ttu-id="013c3-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-176">developer</span><span class="sxs-lookup"><span data-stu-id="013c3-176">developer</span></span>|<span data-ttu-id="013c3-177">String</span><span class="sxs-lookup"><span data-stu-id="013c3-177">String</span></span>|<span data-ttu-id="013c3-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-178">The developer of the app.</span></span> <span data-ttu-id="013c3-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-180">notes</span><span class="sxs-lookup"><span data-stu-id="013c3-180">notes</span></span>|<span data-ttu-id="013c3-181">String</span><span class="sxs-lookup"><span data-stu-id="013c3-181">String</span></span>|<span data-ttu-id="013c3-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="013c3-182">Notes for the app.</span></span> <span data-ttu-id="013c3-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="013c3-184">uploadState</span></span>|<span data-ttu-id="013c3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="013c3-185">Int32</span></span>|<span data-ttu-id="013c3-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="013c3-186">The upload state.</span></span> <span data-ttu-id="013c3-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="013c3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="013c3-188">publishingState</span></span>|[<span data-ttu-id="013c3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="013c3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="013c3-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="013c3-190">The publishing state for the app.</span></span> <span data-ttu-id="013c3-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="013c3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="013c3-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="013c3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="013c3-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="013c3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="013c3-194">packageId</span><span class="sxs-lookup"><span data-stu-id="013c3-194">packageId</span></span>|<span data-ttu-id="013c3-195">String</span><span class="sxs-lookup"><span data-stu-id="013c3-195">String</span></span>|<span data-ttu-id="013c3-196">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="013c3-196">The package identifier.</span></span>|
|<span data-ttu-id="013c3-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="013c3-197">appIdentifier</span></span>|<span data-ttu-id="013c3-198">String</span><span class="sxs-lookup"><span data-stu-id="013c3-198">String</span></span>|<span data-ttu-id="013c3-199">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="013c3-199">The Identity Name.</span></span>|
|<span data-ttu-id="013c3-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="013c3-200">usedLicenseCount</span></span>|<span data-ttu-id="013c3-201">Int32</span><span class="sxs-lookup"><span data-stu-id="013c3-201">Int32</span></span>|<span data-ttu-id="013c3-202">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="013c3-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="013c3-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="013c3-203">totalLicenseCount</span></span>|<span data-ttu-id="013c3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="013c3-204">Int32</span></span>|<span data-ttu-id="013c3-205">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="013c3-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="013c3-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="013c3-206">appStoreUrl</span></span>|<span data-ttu-id="013c3-207">String</span><span class="sxs-lookup"><span data-stu-id="013c3-207">String</span></span>|<span data-ttu-id="013c3-208">Воспроизведение для URL-адреса приложения рабочих хранилища.</span><span class="sxs-lookup"><span data-stu-id="013c3-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="013c3-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="013c3-209">Response</span></span>
<span data-ttu-id="013c3-210">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="013c3-210">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="013c3-211">Пример</span><span class="sxs-lookup"><span data-stu-id="013c3-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="013c3-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="013c3-212">Request</span></span>
<span data-ttu-id="013c3-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="013c3-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="013c3-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="013c3-214">Response</span></span>
<span data-ttu-id="013c3-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="013c3-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 963

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





