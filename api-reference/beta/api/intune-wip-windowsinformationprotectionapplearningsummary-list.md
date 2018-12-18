---
title: Список объектов windowsInformationProtectionAppLearningSummary
description: Список свойств и связей объектов windowsInformationProtectionAppLearningSummary.
author: tfitzmac
ms.openlocfilehash: fd3056eeb82dace50a5c7ab0112b14d6871022ab
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323816"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="325c6-103">Список объектов windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="325c6-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="325c6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="325c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="325c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="325c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="325c6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="325c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="325c6-107">Список свойств и связей объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="325c6-107">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="325c6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="325c6-108">Prerequisites</span></span>
<span data-ttu-id="325c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="325c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="325c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="325c6-111">Permission type</span></span>|<span data-ttu-id="325c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="325c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="325c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="325c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="325c6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="325c6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="325c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="325c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="325c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="325c6-116">Not supported.</span></span>|
|<span data-ttu-id="325c6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="325c6-117">Application</span></span>|<span data-ttu-id="325c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="325c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="325c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="325c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="325c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="325c6-120">Request headers</span></span>
|<span data-ttu-id="325c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="325c6-121">Header</span></span>|<span data-ttu-id="325c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="325c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="325c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="325c6-123">Authorization</span></span>|<span data-ttu-id="325c6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="325c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="325c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="325c6-125">Accept</span></span>|<span data-ttu-id="325c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="325c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="325c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="325c6-127">Request body</span></span>
<span data-ttu-id="325c6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="325c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="325c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="325c6-129">Response</span></span>
<span data-ttu-id="325c6-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="325c6-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="325c6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="325c6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="325c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="325c6-132">Request</span></span>
<span data-ttu-id="325c6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="325c6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="325c6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="325c6-134">Response</span></span>
<span data-ttu-id="325c6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="325c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





