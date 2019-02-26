---
title: Update webApp
description: Обновление свойств объекта webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c645c8dbdd60475215da25e52bfdeeb8ba6e29e0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263289"
---
# <a name="update-webapp"></a><span data-ttu-id="b0963-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="b0963-103">Update webApp</span></span>

> <span data-ttu-id="b0963-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0963-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0963-105">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-105">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0963-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b0963-106">Prerequisites</span></span>
<span data-ttu-id="b0963-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0963-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0963-109">Permission type</span></span>|<span data-ttu-id="b0963-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0963-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0963-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0963-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0963-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0963-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0963-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0963-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0963-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0963-114">Not supported.</span></span>|
|<span data-ttu-id="b0963-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0963-115">Application</span></span>|<span data-ttu-id="b0963-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0963-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0963-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0963-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b0963-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0963-118">Request headers</span></span>
|<span data-ttu-id="b0963-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0963-119">Header</span></span>|<span data-ttu-id="b0963-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b0963-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0963-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0963-121">Authorization</span></span>|<span data-ttu-id="b0963-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b0963-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0963-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b0963-123">Accept</span></span>|<span data-ttu-id="b0963-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0963-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0963-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0963-125">Request body</span></span>
<span data-ttu-id="b0963-126">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0963-126">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="b0963-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-127">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="b0963-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0963-128">Property</span></span>|<span data-ttu-id="b0963-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b0963-129">Type</span></span>|<span data-ttu-id="b0963-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b0963-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0963-131">id</span><span class="sxs-lookup"><span data-stu-id="b0963-131">id</span></span>|<span data-ttu-id="b0963-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b0963-132">String</span></span>|<span data-ttu-id="b0963-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b0963-133">Key of the entity.</span></span> <span data-ttu-id="b0963-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b0963-135">displayName</span></span>|<span data-ttu-id="b0963-136">String</span><span class="sxs-lookup"><span data-stu-id="b0963-136">String</span></span>|<span data-ttu-id="b0963-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b0963-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b0963-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-139">description</span><span class="sxs-lookup"><span data-stu-id="b0963-139">description</span></span>|<span data-ttu-id="b0963-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b0963-140">String</span></span>|<span data-ttu-id="b0963-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-141">The description of the app.</span></span> <span data-ttu-id="b0963-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-143">publisher</span><span class="sxs-lookup"><span data-stu-id="b0963-143">publisher</span></span>|<span data-ttu-id="b0963-144">String</span><span class="sxs-lookup"><span data-stu-id="b0963-144">String</span></span>|<span data-ttu-id="b0963-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-145">The publisher of the app.</span></span> <span data-ttu-id="b0963-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b0963-147">largeIcon</span></span>|[<span data-ttu-id="b0963-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b0963-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b0963-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b0963-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b0963-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0963-151">createdDateTime</span></span>|<span data-ttu-id="b0963-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0963-152">DateTimeOffset</span></span>|<span data-ttu-id="b0963-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-153">The date and time the app was created.</span></span> <span data-ttu-id="b0963-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0963-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b0963-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0963-156">DateTimeOffset</span></span>|<span data-ttu-id="b0963-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b0963-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b0963-159">isFeatured</span></span>|<span data-ttu-id="b0963-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0963-160">Boolean</span></span>|<span data-ttu-id="b0963-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b0963-162">privacyInformationUrl</span></span>|<span data-ttu-id="b0963-163">String</span><span class="sxs-lookup"><span data-stu-id="b0963-163">String</span></span>|<span data-ttu-id="b0963-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b0963-164">The privacy statement Url.</span></span> <span data-ttu-id="b0963-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b0963-166">informationUrl</span></span>|<span data-ttu-id="b0963-167">String</span><span class="sxs-lookup"><span data-stu-id="b0963-167">String</span></span>|<span data-ttu-id="b0963-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b0963-168">The more information Url.</span></span> <span data-ttu-id="b0963-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-170">owner</span><span class="sxs-lookup"><span data-stu-id="b0963-170">owner</span></span>|<span data-ttu-id="b0963-171">Строка</span><span class="sxs-lookup"><span data-stu-id="b0963-171">String</span></span>|<span data-ttu-id="b0963-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-172">The owner of the app.</span></span> <span data-ttu-id="b0963-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-174">developer</span><span class="sxs-lookup"><span data-stu-id="b0963-174">developer</span></span>|<span data-ttu-id="b0963-175">String</span><span class="sxs-lookup"><span data-stu-id="b0963-175">String</span></span>|<span data-ttu-id="b0963-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-176">The developer of the app.</span></span> <span data-ttu-id="b0963-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-178">notes</span><span class="sxs-lookup"><span data-stu-id="b0963-178">notes</span></span>|<span data-ttu-id="b0963-179">String</span><span class="sxs-lookup"><span data-stu-id="b0963-179">String</span></span>|<span data-ttu-id="b0963-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="b0963-180">Notes for the app.</span></span> <span data-ttu-id="b0963-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0963-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b0963-182">publishingState</span></span>|[<span data-ttu-id="b0963-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b0963-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b0963-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-184">The publishing state for the app.</span></span> <span data-ttu-id="b0963-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b0963-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b0963-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0963-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b0963-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b0963-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b0963-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="b0963-188">appUrl</span></span>|<span data-ttu-id="b0963-189">String</span><span class="sxs-lookup"><span data-stu-id="b0963-189">String</span></span>|<span data-ttu-id="b0963-190">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="b0963-190">The web app URL.</span></span>|
|<span data-ttu-id="b0963-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="b0963-191">useManagedBrowser</span></span>|<span data-ttu-id="b0963-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0963-192">Boolean</span></span>|<span data-ttu-id="b0963-193">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="b0963-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="b0963-194">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="b0963-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="b0963-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0963-195">Response</span></span>
<span data-ttu-id="b0963-196">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0963-196">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0963-197">Пример</span><span class="sxs-lookup"><span data-stu-id="b0963-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0963-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0963-198">Request</span></span>
<span data-ttu-id="b0963-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0963-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="b0963-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0963-200">Response</span></span>
<span data-ttu-id="b0963-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b0963-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



