---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abfbae5b425edc1c3ac04989045ebfe1a65f51d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516456"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="7106c-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="7106c-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="7106c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7106c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7106c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7106c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7106c-106">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7106c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7106c-107">Prerequisites</span></span>
<span data-ttu-id="7106c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7106c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7106c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7106c-110">Permission type</span></span>|<span data-ttu-id="7106c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7106c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7106c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7106c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7106c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7106c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7106c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7106c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7106c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7106c-115">Not supported.</span></span>|
|<span data-ttu-id="7106c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7106c-116">Application</span></span>|<span data-ttu-id="7106c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7106c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7106c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7106c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7106c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7106c-119">Request headers</span></span>
|<span data-ttu-id="7106c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7106c-120">Header</span></span>|<span data-ttu-id="7106c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7106c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7106c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7106c-122">Authorization</span></span>|<span data-ttu-id="7106c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7106c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7106c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7106c-124">Accept</span></span>|<span data-ttu-id="7106c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7106c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7106c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7106c-126">Request body</span></span>
<span data-ttu-id="7106c-127">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7106c-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="7106c-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="7106c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7106c-129">Property</span></span>|<span data-ttu-id="7106c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7106c-130">Type</span></span>|<span data-ttu-id="7106c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7106c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7106c-132">id</span><span class="sxs-lookup"><span data-stu-id="7106c-132">id</span></span>|<span data-ttu-id="7106c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-133">String</span></span>|<span data-ttu-id="7106c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7106c-134">Key of the entity.</span></span> <span data-ttu-id="7106c-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7106c-136">displayName</span></span>|<span data-ttu-id="7106c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-137">String</span></span>|<span data-ttu-id="7106c-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7106c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7106c-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-140">description</span><span class="sxs-lookup"><span data-stu-id="7106c-140">description</span></span>|<span data-ttu-id="7106c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-141">String</span></span>|<span data-ttu-id="7106c-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-142">The description of the app.</span></span> <span data-ttu-id="7106c-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7106c-144">publisher</span></span>|<span data-ttu-id="7106c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-145">String</span></span>|<span data-ttu-id="7106c-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-146">The publisher of the app.</span></span> <span data-ttu-id="7106c-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7106c-148">largeIcon</span></span>|[<span data-ttu-id="7106c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7106c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7106c-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7106c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7106c-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7106c-152">createdDateTime</span></span>|<span data-ttu-id="7106c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7106c-153">DateTimeOffset</span></span>|<span data-ttu-id="7106c-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-154">The date and time the app was created.</span></span> <span data-ttu-id="7106c-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7106c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7106c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7106c-157">DateTimeOffset</span></span>|<span data-ttu-id="7106c-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7106c-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7106c-160">isFeatured</span></span>|<span data-ttu-id="7106c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7106c-161">Boolean</span></span>|<span data-ttu-id="7106c-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7106c-163">privacyInformationUrl</span></span>|<span data-ttu-id="7106c-164">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-164">String</span></span>|<span data-ttu-id="7106c-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7106c-165">The privacy statement Url.</span></span> <span data-ttu-id="7106c-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7106c-167">informationUrl</span></span>|<span data-ttu-id="7106c-168">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-168">String</span></span>|<span data-ttu-id="7106c-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7106c-169">The more information Url.</span></span> <span data-ttu-id="7106c-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-171">owner</span><span class="sxs-lookup"><span data-stu-id="7106c-171">owner</span></span>|<span data-ttu-id="7106c-172">String</span><span class="sxs-lookup"><span data-stu-id="7106c-172">String</span></span>|<span data-ttu-id="7106c-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-173">The owner of the app.</span></span> <span data-ttu-id="7106c-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-175">developer</span><span class="sxs-lookup"><span data-stu-id="7106c-175">developer</span></span>|<span data-ttu-id="7106c-176">Строка</span><span class="sxs-lookup"><span data-stu-id="7106c-176">String</span></span>|<span data-ttu-id="7106c-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-177">The developer of the app.</span></span> <span data-ttu-id="7106c-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-179">notes</span><span class="sxs-lookup"><span data-stu-id="7106c-179">notes</span></span>|<span data-ttu-id="7106c-180">String</span><span class="sxs-lookup"><span data-stu-id="7106c-180">String</span></span>|<span data-ttu-id="7106c-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-181">Notes for the app.</span></span> <span data-ttu-id="7106c-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7106c-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="7106c-183">publishingState</span></span>|[<span data-ttu-id="7106c-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7106c-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7106c-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7106c-185">The publishing state for the app.</span></span> <span data-ttu-id="7106c-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7106c-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7106c-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7106c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7106c-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7106c-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="7106c-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="7106c-189">Response</span></span>
<span data-ttu-id="7106c-190">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7106c-190">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7106c-191">Пример</span><span class="sxs-lookup"><span data-stu-id="7106c-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="7106c-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="7106c-192">Request</span></span>
<span data-ttu-id="7106c-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7106c-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="7106c-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="7106c-194">Response</span></span>
<span data-ttu-id="7106c-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7106c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

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
  "publishingState": "processing"
}
```




