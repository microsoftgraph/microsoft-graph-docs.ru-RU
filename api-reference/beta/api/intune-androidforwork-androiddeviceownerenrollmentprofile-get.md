---
title: Получение androidDeviceOwnerEnrollmentProfile
description: Чтение свойства и связи объекта androidDeviceOwnerEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6947171c5d7a366cc5c5fab30bf3143e002c92a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818601"
---
# <a name="get-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="45e3c-103">Получение androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="45e3c-103">Get androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="45e3c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45e3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45e3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45e3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45e3c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45e3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45e3c-107">Чтение свойства и связи объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45e3c-107">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45e3c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45e3c-108">Prerequisites</span></span>
<span data-ttu-id="45e3c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45e3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45e3c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45e3c-111">Permission type</span></span>|<span data-ttu-id="45e3c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45e3c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45e3c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45e3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45e3c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45e3c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45e3c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45e3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45e3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45e3c-116">Not supported.</span></span>|
|<span data-ttu-id="45e3c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45e3c-117">Application</span></span>|<span data-ttu-id="45e3c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45e3c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45e3c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45e3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45e3c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45e3c-120">Optional query parameters</span></span>
<span data-ttu-id="45e3c-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45e3c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45e3c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45e3c-122">Request headers</span></span>
|<span data-ttu-id="45e3c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45e3c-123">Header</span></span>|<span data-ttu-id="45e3c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="45e3c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45e3c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="45e3c-125">Authorization</span></span>|<span data-ttu-id="45e3c-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45e3c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45e3c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="45e3c-127">Accept</span></span>|<span data-ttu-id="45e3c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="45e3c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45e3c-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45e3c-129">Request body</span></span>
<span data-ttu-id="45e3c-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45e3c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45e3c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="45e3c-131">Response</span></span>
<span data-ttu-id="45e3c-132">Успешно завершена, этот метод возвращает `200 OK` объект [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45e3c-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45e3c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="45e3c-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="45e3c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="45e3c-134">Request</span></span>
<span data-ttu-id="45e3c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45e3c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="45e3c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="45e3c-136">Response</span></span>
<span data-ttu-id="45e3c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45e3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
    "accountId": "Account Id value",
    "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "tokenValue": "Token Value value",
    "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "enrolledDeviceCount": 3,
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```





