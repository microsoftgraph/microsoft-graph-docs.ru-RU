---
title: функция managedDeviceEnrollmentFailureTrends
description: Метаданные для отчета тенденций сбой подачи заявок
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c115ee0ada2297c237db839049f9cd33cb77e2ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853490"
---
# <a name="manageddeviceenrollmentfailuretrends-function"></a><span data-ttu-id="3c732-103">функция managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="3c732-103">managedDeviceEnrollmentFailureTrends function</span></span>

> <span data-ttu-id="3c732-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c732-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c732-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c732-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c732-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c732-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c732-107">Метаданные для отчета тенденций сбой подачи заявок</span><span class="sxs-lookup"><span data-stu-id="3c732-107">Metadata for the enrollment failure trends report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3c732-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3c732-108">Prerequisites</span></span>
<span data-ttu-id="3c732-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c732-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c732-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c732-111">Permission type</span></span>|<span data-ttu-id="3c732-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c732-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c732-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c732-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3c732-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="3c732-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3c732-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c732-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3c732-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c732-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c732-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c732-117">Not supported.</span></span>|
|<span data-ttu-id="3c732-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c732-118">Application</span></span>|<span data-ttu-id="3c732-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c732-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c732-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c732-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureTrends
```

## <a name="request-headers"></a><span data-ttu-id="3c732-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c732-121">Request headers</span></span>
|<span data-ttu-id="3c732-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c732-122">Header</span></span>|<span data-ttu-id="3c732-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3c732-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c732-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c732-124">Authorization</span></span>|<span data-ttu-id="3c732-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c732-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c732-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3c732-126">Accept</span></span>|<span data-ttu-id="3c732-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3c732-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c732-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c732-128">Request body</span></span>
<span data-ttu-id="3c732-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c732-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c732-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c732-130">Response</span></span>
<span data-ttu-id="3c732-131">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c732-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c732-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3c732-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c732-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c732-133">Request</span></span>
<span data-ttu-id="3c732-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c732-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureTrends
```

### <a name="response"></a><span data-ttu-id="3c732-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c732-135">Response</span></span>
<span data-ttu-id="3c732-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c732-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



