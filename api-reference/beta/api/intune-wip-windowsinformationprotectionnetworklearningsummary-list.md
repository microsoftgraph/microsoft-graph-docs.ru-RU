---
title: Список объектов windowsInformationProtectionNetworkLearningSummary
description: Список свойств и связей объектов windowsInformationProtectionNetworkLearningSummary.
ms.openlocfilehash: ce9ff2e2fb662408f911cb907f22a7dc72aede72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078010"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="71588-103">Список объектов windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="71588-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

> <span data-ttu-id="71588-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71588-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71588-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71588-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71588-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71588-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71588-107">Список свойств и связей объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="71588-107">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71588-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71588-108">Prerequisites</span></span>
<span data-ttu-id="71588-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71588-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71588-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71588-111">Permission type</span></span>|<span data-ttu-id="71588-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71588-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71588-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71588-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71588-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="71588-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="71588-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71588-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71588-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71588-116">Not supported.</span></span>|
|<span data-ttu-id="71588-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71588-117">Application</span></span>|<span data-ttu-id="71588-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71588-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71588-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71588-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="71588-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71588-120">Request headers</span></span>
|<span data-ttu-id="71588-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71588-121">Header</span></span>|<span data-ttu-id="71588-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71588-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71588-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71588-123">Authorization</span></span>|<span data-ttu-id="71588-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71588-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71588-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71588-125">Accept</span></span>|<span data-ttu-id="71588-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71588-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71588-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71588-127">Request body</span></span>
<span data-ttu-id="71588-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71588-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71588-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="71588-129">Response</span></span>
<span data-ttu-id="71588-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71588-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71588-131">Пример</span><span class="sxs-lookup"><span data-stu-id="71588-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="71588-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71588-132">Request</span></span>
<span data-ttu-id="71588-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71588-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="71588-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="71588-134">Response</span></span>
<span data-ttu-id="71588-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="71588-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
      "id": "242108f7-08f7-2421-f708-2124f7082124",
      "url": "Url value",
      "deviceCount": 11
    }
  ]
}
```





