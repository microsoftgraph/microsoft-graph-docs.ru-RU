---
title: Get deviceCompliancePolicy
description: Чтение свойств и связей объекта deviceCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b58b791781382cce5a0aaf9c2a5ff1ac53997dd1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968499"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="001c2-103">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="001c2-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="001c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="001c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="001c2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="001c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="001c2-106">Чтение свойств и связей объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="001c2-106">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="001c2-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="001c2-107">Prerequisites</span></span>
<span data-ttu-id="001c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="001c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="001c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="001c2-110">Permission type</span></span>|<span data-ttu-id="001c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="001c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="001c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="001c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="001c2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="001c2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="001c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="001c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="001c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="001c2-115">Not supported.</span></span>|
|<span data-ttu-id="001c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="001c2-116">Application</span></span>|<span data-ttu-id="001c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="001c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="001c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="001c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="001c2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="001c2-119">Optional query parameters</span></span>
<span data-ttu-id="001c2-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="001c2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="001c2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="001c2-121">Request headers</span></span>
|<span data-ttu-id="001c2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="001c2-122">Header</span></span>|<span data-ttu-id="001c2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="001c2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="001c2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="001c2-124">Authorization</span></span>|<span data-ttu-id="001c2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="001c2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="001c2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="001c2-126">Accept</span></span>|<span data-ttu-id="001c2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="001c2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="001c2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="001c2-128">Request body</span></span>
<span data-ttu-id="001c2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="001c2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="001c2-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="001c2-130">Response</span></span>
<span data-ttu-id="001c2-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="001c2-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="001c2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="001c2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="001c2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="001c2-133">Request</span></span>
<span data-ttu-id="001c2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="001c2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="001c2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="001c2-135">Response</span></span>
<span data-ttu-id="001c2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="001c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4214b716-b716-4214-16b7-144216b71442",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```





