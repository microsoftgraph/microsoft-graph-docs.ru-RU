---
title: Получение networkIPv4ConfigurationManagementCondition
description: Чтение свойства и связи объекта networkIPv4ConfigurationManagementCondition.
ms.openlocfilehash: ab6b216b031b457206440f3b01ffffdf7e325248
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080423"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="98999-103">Получение networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="98999-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="98999-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98999-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98999-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98999-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98999-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98999-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98999-107">Чтение свойства и связи объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="98999-107">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98999-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98999-108">Prerequisites</span></span>
<span data-ttu-id="98999-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98999-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98999-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98999-111">Permission type</span></span>|<span data-ttu-id="98999-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98999-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98999-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98999-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98999-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="98999-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="98999-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98999-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98999-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98999-116">Not supported.</span></span>|
|<span data-ttu-id="98999-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98999-117">Application</span></span>|<span data-ttu-id="98999-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98999-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98999-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98999-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98999-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98999-120">Optional query parameters</span></span>
<span data-ttu-id="98999-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="98999-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="98999-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98999-122">Request headers</span></span>
|<span data-ttu-id="98999-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98999-123">Header</span></span>|<span data-ttu-id="98999-124">Значение</span><span class="sxs-lookup"><span data-stu-id="98999-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98999-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="98999-125">Authorization</span></span>|<span data-ttu-id="98999-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="98999-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98999-127">Accept</span><span class="sxs-lookup"><span data-stu-id="98999-127">Accept</span></span>|<span data-ttu-id="98999-128">application/json</span><span class="sxs-lookup"><span data-stu-id="98999-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98999-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98999-129">Request body</span></span>
<span data-ttu-id="98999-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98999-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98999-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="98999-131">Response</span></span>
<span data-ttu-id="98999-132">Успешно завершена, этот метод возвращает `200 OK` объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98999-132">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98999-133">Пример</span><span class="sxs-lookup"><span data-stu-id="98999-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="98999-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="98999-134">Request</span></span>
<span data-ttu-id="98999-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98999-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="98999-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="98999-136">Response</span></span>
<span data-ttu-id="98999-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="98999-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
    "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV4Prefix": "Ip V4Prefix value",
    "ipV4Gateway": "Ip V4Gateway value",
    "ipV4DHCPServer": "Ip V4DHCPServer value",
    "ipV4DNSServerList": [
      "Ip V4DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```





