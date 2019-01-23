---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c96761ce5889c8385630b59b3f2a536f0d704
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410653"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="fa6d7-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="fa6d7-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="fa6d7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa6d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa6d7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa6d7-107">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa6d7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fa6d7-108">Prerequisites</span></span>
<span data-ttu-id="fa6d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa6d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa6d7-111">Permission type</span></span>|<span data-ttu-id="fa6d7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa6d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa6d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa6d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa6d7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa6d7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa6d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa6d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa6d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-116">Not supported.</span></span>|
|<span data-ttu-id="fa6d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa6d7-117">Application</span></span>|<span data-ttu-id="fa6d7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa6d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa6d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="fa6d7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa6d7-120">Request headers</span></span>
|<span data-ttu-id="fa6d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa6d7-121">Header</span></span>|<span data-ttu-id="fa6d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa6d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa6d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa6d7-123">Authorization</span></span>|<span data-ttu-id="fa6d7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fa6d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa6d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa6d7-125">Accept</span></span>|<span data-ttu-id="fa6d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa6d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa6d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa6d7-127">Request body</span></span>
<span data-ttu-id="fa6d7-128">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="fa6d7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="fa6d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa6d7-130">Property</span></span>|<span data-ttu-id="fa6d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa6d7-131">Type</span></span>|<span data-ttu-id="fa6d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa6d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa6d7-133">id</span><span class="sxs-lookup"><span data-stu-id="fa6d7-133">id</span></span>|<span data-ttu-id="fa6d7-134">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-134">String</span></span>|<span data-ttu-id="fa6d7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-135">Key of the entity.</span></span> <span data-ttu-id="fa6d7-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fa6d7-137">displayName</span></span>|<span data-ttu-id="fa6d7-138">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-138">String</span></span>|<span data-ttu-id="fa6d7-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fa6d7-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-141">description</span><span class="sxs-lookup"><span data-stu-id="fa6d7-141">description</span></span>|<span data-ttu-id="fa6d7-142">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-142">String</span></span>|<span data-ttu-id="fa6d7-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-143">The description of the app.</span></span> <span data-ttu-id="fa6d7-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fa6d7-145">publisher</span></span>|<span data-ttu-id="fa6d7-146">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-146">String</span></span>|<span data-ttu-id="fa6d7-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-147">The publisher of the app.</span></span> <span data-ttu-id="fa6d7-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fa6d7-149">largeIcon</span></span>|[<span data-ttu-id="fa6d7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fa6d7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fa6d7-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fa6d7-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa6d7-153">createdDateTime</span></span>|<span data-ttu-id="fa6d7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa6d7-154">DateTimeOffset</span></span>|<span data-ttu-id="fa6d7-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-155">The date and time the app was created.</span></span> <span data-ttu-id="fa6d7-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa6d7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fa6d7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa6d7-158">DateTimeOffset</span></span>|<span data-ttu-id="fa6d7-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fa6d7-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fa6d7-161">isFeatured</span></span>|<span data-ttu-id="fa6d7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa6d7-162">Boolean</span></span>|<span data-ttu-id="fa6d7-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fa6d7-164">privacyInformationUrl</span></span>|<span data-ttu-id="fa6d7-165">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-165">String</span></span>|<span data-ttu-id="fa6d7-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-166">The privacy statement Url.</span></span> <span data-ttu-id="fa6d7-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fa6d7-168">informationUrl</span></span>|<span data-ttu-id="fa6d7-169">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-169">String</span></span>|<span data-ttu-id="fa6d7-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-170">The more information Url.</span></span> <span data-ttu-id="fa6d7-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-172">owner</span><span class="sxs-lookup"><span data-stu-id="fa6d7-172">owner</span></span>|<span data-ttu-id="fa6d7-173">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-173">String</span></span>|<span data-ttu-id="fa6d7-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-174">The owner of the app.</span></span> <span data-ttu-id="fa6d7-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-176">developer</span><span class="sxs-lookup"><span data-stu-id="fa6d7-176">developer</span></span>|<span data-ttu-id="fa6d7-177">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-177">String</span></span>|<span data-ttu-id="fa6d7-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-178">The developer of the app.</span></span> <span data-ttu-id="fa6d7-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-180">notes</span><span class="sxs-lookup"><span data-stu-id="fa6d7-180">notes</span></span>|<span data-ttu-id="fa6d7-181">String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-181">String</span></span>|<span data-ttu-id="fa6d7-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-182">Notes for the app.</span></span> <span data-ttu-id="fa6d7-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fa6d7-184">uploadState</span></span>|<span data-ttu-id="fa6d7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fa6d7-185">Int32</span></span>|<span data-ttu-id="fa6d7-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-186">The upload state.</span></span> <span data-ttu-id="fa6d7-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="fa6d7-188">publishingState</span></span>|[<span data-ttu-id="fa6d7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fa6d7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fa6d7-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-190">The publishing state for the app.</span></span> <span data-ttu-id="fa6d7-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fa6d7-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fa6d7-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fa6d7-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fa6d7-194">isAssigned</span></span>|<span data-ttu-id="fa6d7-195">Логический</span><span class="sxs-lookup"><span data-stu-id="fa6d7-195">Boolean</span></span>|<span data-ttu-id="fa6d7-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fa6d7-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fa6d7-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fa6d7-198">roleScopeTagIds</span></span>|<span data-ttu-id="fa6d7-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa6d7-199">String collection</span></span>|<span data-ttu-id="fa6d7-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fa6d7-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa6d7-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="fa6d7-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa6d7-202">Response</span></span>
<span data-ttu-id="fa6d7-203">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-203">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa6d7-204">Пример</span><span class="sxs-lookup"><span data-stu-id="fa6d7-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa6d7-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa6d7-205">Request</span></span>
<span data-ttu-id="fa6d7-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 691

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fa6d7-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa6d7-207">Response</span></span>
<span data-ttu-id="fa6d7-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fa6d7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




