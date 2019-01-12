---
title: Действие consentToDataSharing
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85a0b7a19fba7fca26916b888c53cf24157ec594
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979441"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="2b6f5-103">Действие consentToDataSharing</span><span class="sxs-lookup"><span data-stu-id="2b6f5-103">consentToDataSharing action</span></span>

> <span data-ttu-id="2b6f5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b6f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b6f5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b6f5-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b6f5-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b6f5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2b6f5-108">Prerequisites</span></span>
<span data-ttu-id="2b6f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b6f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b6f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b6f5-111">Permission type</span></span>|<span data-ttu-id="2b6f5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b6f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b6f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6f5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6f5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2b6f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b6f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-116">Not supported.</span></span>|
|<span data-ttu-id="2b6f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b6f5-117">Application</span></span>|<span data-ttu-id="2b6f5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b6f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="2b6f5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b6f5-120">Request headers</span></span>
|<span data-ttu-id="2b6f5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b6f5-121">Header</span></span>|<span data-ttu-id="2b6f5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b6f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b6f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b6f5-123">Authorization</span></span>|<span data-ttu-id="2b6f5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b6f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b6f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b6f5-125">Accept</span></span>|<span data-ttu-id="2b6f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b6f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6f5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b6f5-127">Request body</span></span>
<span data-ttu-id="2b6f5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b6f5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b6f5-129">Response</span></span>
<span data-ttu-id="2b6f5-130">Если успешно завершена, это действие возвращает `200 OK` код ответа и [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-130">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b6f5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2b6f5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b6f5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b6f5-132">Request</span></span>
<span data-ttu-id="2b6f5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="2b6f5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b6f5-134">Response</span></span>
<span data-ttu-id="2b6f5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b6f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```





