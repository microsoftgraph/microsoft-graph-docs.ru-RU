---
title: Список объектов windowsInformationProtectionNetworkLearningSummary
description: Список свойств и связей объектов windowsInformationProtectionNetworkLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fe13b40ecd00114e03978f5a3a828795fb0622a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263114"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="cdca4-103">Список объектов windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="cdca4-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

> <span data-ttu-id="cdca4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdca4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdca4-105">Список свойств и связей объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cdca4-105">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdca4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cdca4-106">Prerequisites</span></span>
<span data-ttu-id="cdca4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cdca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cdca4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdca4-109">Permission type</span></span>|<span data-ttu-id="cdca4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdca4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdca4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdca4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdca4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdca4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cdca4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdca4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdca4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdca4-114">Not supported.</span></span>|
|<span data-ttu-id="cdca4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdca4-115">Application</span></span>|<span data-ttu-id="cdca4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdca4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdca4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdca4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="cdca4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdca4-118">Request headers</span></span>
|<span data-ttu-id="cdca4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdca4-119">Header</span></span>|<span data-ttu-id="cdca4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cdca4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdca4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdca4-121">Authorization</span></span>|<span data-ttu-id="cdca4-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cdca4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdca4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cdca4-123">Accept</span></span>|<span data-ttu-id="cdca4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdca4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdca4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdca4-125">Request body</span></span>
<span data-ttu-id="cdca4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdca4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdca4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdca4-127">Response</span></span>
<span data-ttu-id="cdca4-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cdca4-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdca4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="cdca4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdca4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdca4-130">Request</span></span>
<span data-ttu-id="cdca4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdca4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="cdca4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdca4-132">Response</span></span>
<span data-ttu-id="cdca4-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cdca4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



