---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 640d92ddc7094ab04759f0cd9ce0ac5cf735f783
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577093"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="9ea4b-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="9ea4b-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="9ea4b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ea4b-105">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-105">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ea4b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9ea4b-106">Prerequisites</span></span>
<span data-ttu-id="9ea4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea4b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea4b-109">Permission type</span></span>|<span data-ttu-id="9ea4b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ea4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ea4b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ea4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ea4b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea4b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ea4b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ea4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ea4b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-114">Not supported.</span></span>|
|<span data-ttu-id="9ea4b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ea4b-115">Application</span></span>|<span data-ttu-id="9ea4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ea4b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ea4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9ea4b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ea4b-118">Request headers</span></span>
|<span data-ttu-id="9ea4b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ea4b-119">Header</span></span>|<span data-ttu-id="9ea4b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9ea4b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ea4b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ea4b-121">Authorization</span></span>|<span data-ttu-id="9ea4b-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ea4b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9ea4b-123">Accept</span></span>|<span data-ttu-id="9ea4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9ea4b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ea4b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ea4b-125">Request body</span></span>
<span data-ttu-id="9ea4b-126">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-126">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="9ea4b-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-127">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="9ea4b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ea4b-128">Property</span></span>|<span data-ttu-id="9ea4b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9ea4b-129">Type</span></span>|<span data-ttu-id="9ea4b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9ea4b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea4b-131">id</span><span class="sxs-lookup"><span data-stu-id="9ea4b-131">id</span></span>|<span data-ttu-id="9ea4b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9ea4b-132">String</span></span>|<span data-ttu-id="9ea4b-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-133">Key of the entity.</span></span> <span data-ttu-id="9ea4b-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9ea4b-135">displayName</span></span>|<span data-ttu-id="9ea4b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="9ea4b-136">String</span></span>|<span data-ttu-id="9ea4b-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ea4b-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-139">description</span><span class="sxs-lookup"><span data-stu-id="9ea4b-139">description</span></span>|<span data-ttu-id="9ea4b-140">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-140">String</span></span>|<span data-ttu-id="9ea4b-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-141">The description of the app.</span></span> <span data-ttu-id="9ea4b-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="9ea4b-143">publisher</span></span>|<span data-ttu-id="9ea4b-144">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-144">String</span></span>|<span data-ttu-id="9ea4b-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-145">The publisher of the app.</span></span> <span data-ttu-id="9ea4b-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ea4b-147">largeIcon</span></span>|[<span data-ttu-id="9ea4b-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ea4b-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ea4b-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ea4b-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ea4b-151">createdDateTime</span></span>|<span data-ttu-id="9ea4b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ea4b-152">DateTimeOffset</span></span>|<span data-ttu-id="9ea4b-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-153">The date and time the app was created.</span></span> <span data-ttu-id="9ea4b-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ea4b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9ea4b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ea4b-156">DateTimeOffset</span></span>|<span data-ttu-id="9ea4b-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-157">The date and time the app was last modified.</span></span> <span data-ttu-id="9ea4b-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ea4b-159">isFeatured</span></span>|<span data-ttu-id="9ea4b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ea4b-160">Boolean</span></span>|<span data-ttu-id="9ea4b-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ea4b-162">privacyInformationUrl</span></span>|<span data-ttu-id="9ea4b-163">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-163">String</span></span>|<span data-ttu-id="9ea4b-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-164">The privacy statement Url.</span></span> <span data-ttu-id="9ea4b-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ea4b-166">informationUrl</span></span>|<span data-ttu-id="9ea4b-167">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-167">String</span></span>|<span data-ttu-id="9ea4b-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-168">The more information Url.</span></span> <span data-ttu-id="9ea4b-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-170">owner</span><span class="sxs-lookup"><span data-stu-id="9ea4b-170">owner</span></span>|<span data-ttu-id="9ea4b-171">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-171">String</span></span>|<span data-ttu-id="9ea4b-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-172">The owner of the app.</span></span> <span data-ttu-id="9ea4b-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-174">developer</span><span class="sxs-lookup"><span data-stu-id="9ea4b-174">developer</span></span>|<span data-ttu-id="9ea4b-175">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-175">String</span></span>|<span data-ttu-id="9ea4b-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-176">The developer of the app.</span></span> <span data-ttu-id="9ea4b-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-178">notes</span><span class="sxs-lookup"><span data-stu-id="9ea4b-178">notes</span></span>|<span data-ttu-id="9ea4b-179">String</span><span class="sxs-lookup"><span data-stu-id="9ea4b-179">String</span></span>|<span data-ttu-id="9ea4b-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-180">Notes for the app.</span></span> <span data-ttu-id="9ea4b-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ea4b-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ea4b-182">publishingState</span></span>|[<span data-ttu-id="9ea4b-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9ea4b-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ea4b-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-184">The publishing state for the app.</span></span> <span data-ttu-id="9ea4b-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ea4b-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ea4b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9ea4b-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ea4b-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea4b-188">Response</span></span>
<span data-ttu-id="9ea4b-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-189">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea4b-190">Пример</span><span class="sxs-lookup"><span data-stu-id="9ea4b-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ea4b-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ea4b-191">Request</span></span>
<span data-ttu-id="9ea4b-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ea4b-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea4b-193">Response</span></span>
<span data-ttu-id="9ea4b-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ea4b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



