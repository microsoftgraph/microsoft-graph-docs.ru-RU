---
title: List deviceComplianceUserStatuses
description: Перечисление свойств и связей объектов deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b1ac8c92c6ae17deec8c10de425907a410f16c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827533"
---
# <a name="list-devicecomplianceuserstatuses"></a><span data-ttu-id="c7e41-103">List deviceComplianceUserStatuses</span><span class="sxs-lookup"><span data-stu-id="c7e41-103">List deviceComplianceUserStatuses</span></span>

> <span data-ttu-id="c7e41-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7e41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7e41-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7e41-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c7e41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7e41-107">Перечисление свойств и связей объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c7e41-107">List properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7e41-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e41-108">Prerequisites</span></span>
<span data-ttu-id="c7e41-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e41-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e41-111">Permission type</span></span>|<span data-ttu-id="c7e41-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7e41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7e41-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7e41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7e41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7e41-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7e41-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7e41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7e41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e41-116">Not supported.</span></span>|
|<span data-ttu-id="c7e41-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7e41-117">Application</span></span>|<span data-ttu-id="c7e41-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7e41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7e41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7e41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c7e41-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7e41-120">Request headers</span></span>
|<span data-ttu-id="c7e41-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7e41-121">Header</span></span>|<span data-ttu-id="c7e41-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7e41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7e41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7e41-123">Authorization</span></span>|<span data-ttu-id="c7e41-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7e41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7e41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7e41-125">Accept</span></span>|<span data-ttu-id="c7e41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7e41-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7e41-127">Request body</span></span>
<span data-ttu-id="c7e41-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7e41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7e41-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7e41-129">Response</span></span>
<span data-ttu-id="c7e41-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7e41-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e41-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c7e41-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7e41-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7e41-132">Request</span></span>
<span data-ttu-id="c7e41-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7e41-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="c7e41-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7e41-134">Response</span></span>
<span data-ttu-id="c7e41-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7e41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 397

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
      "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





