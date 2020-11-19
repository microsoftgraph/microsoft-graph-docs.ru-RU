---
title: Список объектов windowsInformationProtectionNetworkLearningSummary
description: Список свойств и связей объектов windowsInformationProtectionNetworkLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ae3f7659432e50bc9cf212bf49b99e366061985
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261372"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="4f61f-103">Список объектов windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="4f61f-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

<span data-ttu-id="4f61f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f61f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f61f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f61f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f61f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f61f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f61f-107">Список свойств и связей объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4f61f-107">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f61f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f61f-108">Prerequisites</span></span>
<span data-ttu-id="4f61f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f61f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f61f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f61f-111">Permission type</span></span>|<span data-ttu-id="4f61f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f61f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f61f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f61f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f61f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f61f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4f61f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f61f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f61f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f61f-116">Not supported.</span></span>|
|<span data-ttu-id="4f61f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f61f-117">Application</span></span>|<span data-ttu-id="4f61f-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f61f-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f61f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f61f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4f61f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f61f-120">Request headers</span></span>
|<span data-ttu-id="4f61f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f61f-121">Header</span></span>|<span data-ttu-id="4f61f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f61f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f61f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f61f-123">Authorization</span></span>|<span data-ttu-id="4f61f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f61f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f61f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f61f-125">Accept</span></span>|<span data-ttu-id="4f61f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f61f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f61f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f61f-127">Request body</span></span>
<span data-ttu-id="4f61f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f61f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f61f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f61f-129">Response</span></span>
<span data-ttu-id="4f61f-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f61f-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f61f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f61f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f61f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f61f-132">Request</span></span>
<span data-ttu-id="4f61f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f61f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="4f61f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f61f-134">Response</span></span>
<span data-ttu-id="4f61f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f61f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




