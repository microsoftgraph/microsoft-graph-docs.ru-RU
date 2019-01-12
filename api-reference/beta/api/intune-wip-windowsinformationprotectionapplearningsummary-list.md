---
title: Список объектов windowsInformationProtectionAppLearningSummary
description: Список свойств и связей объектов windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42c5c29f952a23b7f5744bc9dbb1de28bb5ee074
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913774"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="40abe-103">Список объектов windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="40abe-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="40abe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40abe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40abe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40abe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40abe-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40abe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40abe-107">Список свойств и связей объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="40abe-107">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40abe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40abe-108">Prerequisites</span></span>
<span data-ttu-id="40abe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40abe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40abe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40abe-111">Permission type</span></span>|<span data-ttu-id="40abe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40abe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40abe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40abe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40abe-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="40abe-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="40abe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40abe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40abe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40abe-116">Not supported.</span></span>|
|<span data-ttu-id="40abe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40abe-117">Application</span></span>|<span data-ttu-id="40abe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40abe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40abe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40abe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="40abe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40abe-120">Request headers</span></span>
|<span data-ttu-id="40abe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40abe-121">Header</span></span>|<span data-ttu-id="40abe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40abe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40abe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40abe-123">Authorization</span></span>|<span data-ttu-id="40abe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="40abe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40abe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40abe-125">Accept</span></span>|<span data-ttu-id="40abe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40abe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40abe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40abe-127">Request body</span></span>
<span data-ttu-id="40abe-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40abe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40abe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="40abe-129">Response</span></span>
<span data-ttu-id="40abe-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40abe-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40abe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="40abe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="40abe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="40abe-132">Request</span></span>
<span data-ttu-id="40abe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40abe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="40abe-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="40abe-134">Response</span></span>
<span data-ttu-id="40abe-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40abe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
      "id": "063baf50-af50-063b-50af-3b0650af3b06",
      "applicationName": "Application Name value",
      "applicationType": "desktop",
      "deviceCount": 11
    }
  ]
}
```





