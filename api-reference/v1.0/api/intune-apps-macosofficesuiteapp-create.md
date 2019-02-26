---
title: Создание объекта macOSOfficeSuiteApp
description: Создание объекта macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2df408fe4c5d571789896a93e7b2387f7263a590
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260454"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="d689d-103">Создание объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="d689d-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="d689d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d689d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d689d-105">Создание объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-105">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d689d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d689d-106">Prerequisites</span></span>
<span data-ttu-id="d689d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d689d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d689d-109">Permission type</span></span>|<span data-ttu-id="d689d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d689d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d689d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d689d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d689d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d689d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d689d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d689d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d689d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d689d-114">Not supported.</span></span>|
|<span data-ttu-id="d689d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d689d-115">Application</span></span>|<span data-ttu-id="d689d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d689d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d689d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d689d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d689d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d689d-118">Request headers</span></span>
|<span data-ttu-id="d689d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d689d-119">Header</span></span>|<span data-ttu-id="d689d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d689d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d689d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d689d-121">Authorization</span></span>|<span data-ttu-id="d689d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d689d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d689d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d689d-123">Accept</span></span>|<span data-ttu-id="d689d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d689d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d689d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d689d-125">Request body</span></span>
<span data-ttu-id="d689d-126">В тексте запроса добавьте представление объекта macOSOfficeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d689d-126">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="d689d-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="d689d-127">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="d689d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d689d-128">Property</span></span>|<span data-ttu-id="d689d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d689d-129">Type</span></span>|<span data-ttu-id="d689d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d689d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d689d-131">id</span><span class="sxs-lookup"><span data-stu-id="d689d-131">id</span></span>|<span data-ttu-id="d689d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d689d-132">String</span></span>|<span data-ttu-id="d689d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d689d-133">Key of the entity.</span></span> <span data-ttu-id="d689d-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d689d-135">displayName</span></span>|<span data-ttu-id="d689d-136">String</span><span class="sxs-lookup"><span data-stu-id="d689d-136">String</span></span>|<span data-ttu-id="d689d-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d689d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d689d-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-139">description</span><span class="sxs-lookup"><span data-stu-id="d689d-139">description</span></span>|<span data-ttu-id="d689d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d689d-140">String</span></span>|<span data-ttu-id="d689d-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-141">The description of the app.</span></span> <span data-ttu-id="d689d-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="d689d-143">publisher</span></span>|<span data-ttu-id="d689d-144">String</span><span class="sxs-lookup"><span data-stu-id="d689d-144">String</span></span>|<span data-ttu-id="d689d-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-145">The publisher of the app.</span></span> <span data-ttu-id="d689d-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d689d-147">largeIcon</span></span>|[<span data-ttu-id="d689d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d689d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d689d-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d689d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d689d-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d689d-151">createdDateTime</span></span>|<span data-ttu-id="d689d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d689d-152">DateTimeOffset</span></span>|<span data-ttu-id="d689d-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-153">The date and time the app was created.</span></span> <span data-ttu-id="d689d-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d689d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d689d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d689d-156">DateTimeOffset</span></span>|<span data-ttu-id="d689d-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="d689d-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d689d-159">isFeatured</span></span>|<span data-ttu-id="d689d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d689d-160">Boolean</span></span>|<span data-ttu-id="d689d-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d689d-162">privacyInformationUrl</span></span>|<span data-ttu-id="d689d-163">String</span><span class="sxs-lookup"><span data-stu-id="d689d-163">String</span></span>|<span data-ttu-id="d689d-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d689d-164">The privacy statement Url.</span></span> <span data-ttu-id="d689d-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d689d-166">informationUrl</span></span>|<span data-ttu-id="d689d-167">String</span><span class="sxs-lookup"><span data-stu-id="d689d-167">String</span></span>|<span data-ttu-id="d689d-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d689d-168">The more information Url.</span></span> <span data-ttu-id="d689d-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-170">owner</span><span class="sxs-lookup"><span data-stu-id="d689d-170">owner</span></span>|<span data-ttu-id="d689d-171">String</span><span class="sxs-lookup"><span data-stu-id="d689d-171">String</span></span>|<span data-ttu-id="d689d-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-172">The owner of the app.</span></span> <span data-ttu-id="d689d-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-174">developer</span><span class="sxs-lookup"><span data-stu-id="d689d-174">developer</span></span>|<span data-ttu-id="d689d-175">String</span><span class="sxs-lookup"><span data-stu-id="d689d-175">String</span></span>|<span data-ttu-id="d689d-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-176">The developer of the app.</span></span> <span data-ttu-id="d689d-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-178">notes</span><span class="sxs-lookup"><span data-stu-id="d689d-178">notes</span></span>|<span data-ttu-id="d689d-179">String</span><span class="sxs-lookup"><span data-stu-id="d689d-179">String</span></span>|<span data-ttu-id="d689d-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="d689d-180">Notes for the app.</span></span> <span data-ttu-id="d689d-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d689d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="d689d-182">publishingState</span></span>|[<span data-ttu-id="d689d-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d689d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d689d-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="d689d-184">The publishing state for the app.</span></span> <span data-ttu-id="d689d-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d689d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d689d-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d689d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d689d-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d689d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="d689d-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="d689d-188">Response</span></span>
<span data-ttu-id="d689d-189">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d689d-189">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d689d-190">Пример</span><span class="sxs-lookup"><span data-stu-id="d689d-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="d689d-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="d689d-191">Request</span></span>
<span data-ttu-id="d689d-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d689d-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d689d-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="d689d-193">Response</span></span>
<span data-ttu-id="d689d-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d689d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



