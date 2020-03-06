---
title: Создание объекта macOSOfficeSuiteApp
description: Создание объекта macOSOfficeSuiteApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78da5f6b9a577b6f3071e23868753d7e25a20a96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516485"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="b1655-103">Создание объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="b1655-103">Create macOSOfficeSuiteApp</span></span>

<span data-ttu-id="b1655-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1655-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1655-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1655-106">Создание объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1655-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1655-107">Prerequisites</span></span>
<span data-ttu-id="b1655-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1655-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1655-110">Permission type</span></span>|<span data-ttu-id="b1655-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1655-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1655-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1655-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1655-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1655-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1655-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1655-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1655-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1655-115">Not supported.</span></span>|
|<span data-ttu-id="b1655-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1655-116">Application</span></span>|<span data-ttu-id="b1655-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1655-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1655-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1655-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b1655-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1655-119">Request headers</span></span>
|<span data-ttu-id="b1655-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1655-120">Header</span></span>|<span data-ttu-id="b1655-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1655-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1655-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1655-122">Authorization</span></span>|<span data-ttu-id="b1655-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1655-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1655-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1655-124">Accept</span></span>|<span data-ttu-id="b1655-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1655-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1655-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1655-126">Request body</span></span>
<span data-ttu-id="b1655-127">В тексте запроса добавьте представление объекта macOSOfficeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1655-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="b1655-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="b1655-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="b1655-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1655-129">Property</span></span>|<span data-ttu-id="b1655-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b1655-130">Type</span></span>|<span data-ttu-id="b1655-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b1655-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1655-132">id</span><span class="sxs-lookup"><span data-stu-id="b1655-132">id</span></span>|<span data-ttu-id="b1655-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-133">String</span></span>|<span data-ttu-id="b1655-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1655-134">Key of the entity.</span></span> <span data-ttu-id="b1655-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b1655-136">displayName</span></span>|<span data-ttu-id="b1655-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-137">String</span></span>|<span data-ttu-id="b1655-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b1655-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b1655-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-140">description</span><span class="sxs-lookup"><span data-stu-id="b1655-140">description</span></span>|<span data-ttu-id="b1655-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-141">String</span></span>|<span data-ttu-id="b1655-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-142">The description of the app.</span></span> <span data-ttu-id="b1655-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b1655-144">publisher</span></span>|<span data-ttu-id="b1655-145">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-145">String</span></span>|<span data-ttu-id="b1655-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-146">The publisher of the app.</span></span> <span data-ttu-id="b1655-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b1655-148">largeIcon</span></span>|[<span data-ttu-id="b1655-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b1655-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b1655-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b1655-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b1655-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1655-152">createdDateTime</span></span>|<span data-ttu-id="b1655-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1655-153">DateTimeOffset</span></span>|<span data-ttu-id="b1655-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-154">The date and time the app was created.</span></span> <span data-ttu-id="b1655-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1655-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b1655-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1655-157">DateTimeOffset</span></span>|<span data-ttu-id="b1655-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b1655-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b1655-160">isFeatured</span></span>|<span data-ttu-id="b1655-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1655-161">Boolean</span></span>|<span data-ttu-id="b1655-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b1655-163">privacyInformationUrl</span></span>|<span data-ttu-id="b1655-164">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-164">String</span></span>|<span data-ttu-id="b1655-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b1655-165">The privacy statement Url.</span></span> <span data-ttu-id="b1655-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b1655-167">informationUrl</span></span>|<span data-ttu-id="b1655-168">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-168">String</span></span>|<span data-ttu-id="b1655-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b1655-169">The more information Url.</span></span> <span data-ttu-id="b1655-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-171">owner</span><span class="sxs-lookup"><span data-stu-id="b1655-171">owner</span></span>|<span data-ttu-id="b1655-172">String</span><span class="sxs-lookup"><span data-stu-id="b1655-172">String</span></span>|<span data-ttu-id="b1655-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-173">The owner of the app.</span></span> <span data-ttu-id="b1655-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-175">developer</span><span class="sxs-lookup"><span data-stu-id="b1655-175">developer</span></span>|<span data-ttu-id="b1655-176">Строка</span><span class="sxs-lookup"><span data-stu-id="b1655-176">String</span></span>|<span data-ttu-id="b1655-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-177">The developer of the app.</span></span> <span data-ttu-id="b1655-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-179">notes</span><span class="sxs-lookup"><span data-stu-id="b1655-179">notes</span></span>|<span data-ttu-id="b1655-180">String</span><span class="sxs-lookup"><span data-stu-id="b1655-180">String</span></span>|<span data-ttu-id="b1655-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-181">Notes for the app.</span></span> <span data-ttu-id="b1655-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b1655-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="b1655-183">publishingState</span></span>|[<span data-ttu-id="b1655-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b1655-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b1655-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b1655-185">The publishing state for the app.</span></span> <span data-ttu-id="b1655-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b1655-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b1655-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1655-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b1655-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b1655-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="b1655-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1655-189">Response</span></span>
<span data-ttu-id="b1655-190">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1655-190">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1655-191">Пример</span><span class="sxs-lookup"><span data-stu-id="b1655-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1655-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1655-192">Request</span></span>
<span data-ttu-id="b1655-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1655-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="b1655-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1655-194">Response</span></span>
<span data-ttu-id="b1655-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1655-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




