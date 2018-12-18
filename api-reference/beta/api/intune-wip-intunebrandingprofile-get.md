---
title: Получение intuneBrandingProfile
description: Чтение свойства и связи объекта intuneBrandingProfile.
author: tfitzmac
ms.openlocfilehash: 2c90dc24f85f6c259c48cdf0ba2e431ef5c8c55a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333574"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="60292-103">Получение intuneBrandingProfile</span><span class="sxs-lookup"><span data-stu-id="60292-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="60292-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="60292-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60292-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60292-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60292-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="60292-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60292-107">Чтение свойства и связи объекта [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="60292-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60292-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="60292-108">Prerequisites</span></span>
<span data-ttu-id="60292-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60292-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60292-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60292-111">Permission type</span></span>|<span data-ttu-id="60292-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="60292-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60292-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60292-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60292-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="60292-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="60292-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60292-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60292-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60292-116">Not supported.</span></span>|
|<span data-ttu-id="60292-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60292-117">Application</span></span>|<span data-ttu-id="60292-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60292-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60292-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60292-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60292-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60292-120">Optional query parameters</span></span>
<span data-ttu-id="60292-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60292-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="60292-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60292-122">Request headers</span></span>
|<span data-ttu-id="60292-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60292-123">Header</span></span>|<span data-ttu-id="60292-124">Значение</span><span class="sxs-lookup"><span data-stu-id="60292-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60292-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60292-125">Authorization</span></span>|<span data-ttu-id="60292-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="60292-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60292-127">Accept</span><span class="sxs-lookup"><span data-stu-id="60292-127">Accept</span></span>|<span data-ttu-id="60292-128">application/json</span><span class="sxs-lookup"><span data-stu-id="60292-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60292-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60292-129">Request body</span></span>
<span data-ttu-id="60292-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60292-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60292-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="60292-131">Response</span></span>
<span data-ttu-id="60292-132">Успешно завершена, этот метод возвращает `200 OK` объект [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="60292-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60292-133">Пример</span><span class="sxs-lookup"><span data-stu-id="60292-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="60292-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="60292-134">Request</span></span>
<span data-ttu-id="60292-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60292-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="60292-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="60292-136">Response</span></span>
<span data-ttu-id="60292-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="60292-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





