---
title: Получение Интунебрандингпрофиле
description: Чтение свойств и связей объекта Интунебрандингпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 554d7ad87f0c5c33e827fbf53b711d96871b434d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174582"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="d7f48-103">Получение Интунебрандингпрофиле</span><span class="sxs-lookup"><span data-stu-id="d7f48-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="d7f48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7f48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7f48-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7f48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7f48-106">Чтение свойств и связей объекта [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d7f48-106">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7f48-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7f48-107">Prerequisites</span></span>
<span data-ttu-id="d7f48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7f48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7f48-110">Permission type</span></span>|<span data-ttu-id="d7f48-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7f48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7f48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7f48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7f48-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7f48-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d7f48-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7f48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7f48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7f48-115">Not supported.</span></span>|
|<span data-ttu-id="d7f48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7f48-116">Application</span></span>|<span data-ttu-id="d7f48-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7f48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7f48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7f48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7f48-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7f48-119">Optional query parameters</span></span>
<span data-ttu-id="d7f48-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7f48-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7f48-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7f48-121">Request headers</span></span>
|<span data-ttu-id="d7f48-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7f48-122">Header</span></span>|<span data-ttu-id="d7f48-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d7f48-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7f48-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7f48-124">Authorization</span></span>|<span data-ttu-id="d7f48-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d7f48-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7f48-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d7f48-126">Accept</span></span>|<span data-ttu-id="d7f48-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d7f48-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7f48-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7f48-128">Request body</span></span>
<span data-ttu-id="d7f48-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7f48-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7f48-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7f48-130">Response</span></span>
<span data-ttu-id="d7f48-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [интунебрандингпрофиле](../resources/intune-wip-intunebrandingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7f48-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7f48-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d7f48-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7f48-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7f48-133">Request</span></span>
<span data-ttu-id="d7f48-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7f48-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="d7f48-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7f48-135">Response</span></span>
<span data-ttu-id="d7f48-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d7f48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1472

{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfile",
    "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
    "profileName": "Profile Name value",
    "profileDescription": "Profile Description value",
    "isDefaultProfile": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "showDisplayNameNextToLogo": true,
    "themeColorLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "landingPageCustomizedImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```




