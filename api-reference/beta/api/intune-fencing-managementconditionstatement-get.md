---
title: Get managementConditionStatement
description: Чтение свойств и связей объекта managementConditionStatement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80dd26ef13bb8fc806fd8a79f0bb87023761955d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153680"
---
# <a name="get-managementconditionstatement"></a><span data-ttu-id="a3748-103">Get managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="a3748-103">Get managementConditionStatement</span></span>

<span data-ttu-id="a3748-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3748-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3748-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3748-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3748-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3748-107">Чтение свойств и связей [объекта managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="a3748-107">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3748-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3748-108">Prerequisites</span></span>
<span data-ttu-id="a3748-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3748-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3748-111">Permission type</span></span>|<span data-ttu-id="a3748-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3748-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3748-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3748-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3748-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3748-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3748-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3748-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3748-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3748-116">Not supported.</span></span>|
|<span data-ttu-id="a3748-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3748-117">Application</span></span>|<span data-ttu-id="a3748-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3748-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3748-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3748-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3748-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3748-120">Optional query parameters</span></span>
<span data-ttu-id="a3748-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3748-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3748-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3748-122">Request headers</span></span>
|<span data-ttu-id="a3748-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3748-123">Header</span></span>|<span data-ttu-id="a3748-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a3748-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3748-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3748-125">Authorization</span></span>|<span data-ttu-id="a3748-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3748-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3748-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a3748-127">Accept</span></span>|<span data-ttu-id="a3748-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a3748-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3748-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3748-129">Request body</span></span>
<span data-ttu-id="a3748-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3748-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3748-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3748-131">Response</span></span>
<span data-ttu-id="a3748-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a3748-132">If successful, this method returns a `200 OK` response code and [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3748-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a3748-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3748-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3748-134">Request</span></span>
<span data-ttu-id="a3748-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3748-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
```

### <a name="response"></a><span data-ttu-id="a3748-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3748-136">Response</span></span>
<span data-ttu-id="a3748-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 573

{
  "value": {
    "@odata.type": "#microsoft.graph.managementConditionStatement",
    "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "expression": {
      "@odata.type": "microsoft.graph.managementConditionExpressionString",
      "value": "Value value"
    },
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```




