---
title: Получение embeddedSIMActivationCodePool
description: Чтение свойства и связи объекта embeddedSIMActivationCodePool.
ms.openlocfilehash: 97752212df207e5c530c785b699382ac8c0f4a64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075862"
---
# <a name="get-embeddedsimactivationcodepool"></a><span data-ttu-id="31895-103">Получение embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="31895-103">Get embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="31895-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31895-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31895-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31895-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31895-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="31895-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31895-107">Чтение свойства и связи объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .</span><span class="sxs-lookup"><span data-stu-id="31895-107">Read properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31895-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31895-108">Prerequisites</span></span>
<span data-ttu-id="31895-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31895-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31895-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31895-111">Permission type</span></span>|<span data-ttu-id="31895-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31895-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31895-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31895-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31895-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="31895-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="31895-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31895-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31895-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31895-116">Not supported.</span></span>|
|<span data-ttu-id="31895-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31895-117">Application</span></span>|<span data-ttu-id="31895-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31895-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31895-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31895-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31895-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31895-120">Optional query parameters</span></span>
<span data-ttu-id="31895-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31895-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="31895-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31895-122">Request headers</span></span>
|<span data-ttu-id="31895-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31895-123">Header</span></span>|<span data-ttu-id="31895-124">Значение</span><span class="sxs-lookup"><span data-stu-id="31895-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31895-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="31895-125">Authorization</span></span>|<span data-ttu-id="31895-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="31895-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31895-127">Accept</span><span class="sxs-lookup"><span data-stu-id="31895-127">Accept</span></span>|<span data-ttu-id="31895-128">application/json</span><span class="sxs-lookup"><span data-stu-id="31895-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31895-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31895-129">Request body</span></span>
<span data-ttu-id="31895-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31895-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31895-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="31895-131">Response</span></span>
<span data-ttu-id="31895-132">Успешно завершена, этот метод возвращает `200 OK` объект [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="31895-132">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31895-133">Пример</span><span class="sxs-lookup"><span data-stu-id="31895-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="31895-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="31895-134">Request</span></span>
<span data-ttu-id="31895-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31895-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

### <a name="response"></a><span data-ttu-id="31895-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="31895-136">Response</span></span>
<span data-ttu-id="31895-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="31895-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
    "id": "ec308741-8741-ec30-4187-30ec418730ec",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "activationCodes": [
      {
        "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
        "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
        "matchingIdentifier": "Matching Identifier value",
        "smdpPlusServerAddress": "Smdp Plus Server Address value"
      }
    ],
    "activationCodeCount": 3
  }
}
```





