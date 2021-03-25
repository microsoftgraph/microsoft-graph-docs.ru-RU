---
title: функция getManagementConditionStatementExpressionString
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0fa93e7fe9d9d2730a5a4711ff0ba52bef5557e6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153652"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="c2895-103">функция getManagementConditionStatementExpressionString</span><span class="sxs-lookup"><span data-stu-id="c2895-103">getManagementConditionStatementExpressionString function</span></span>

<span data-ttu-id="c2895-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2895-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2895-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2895-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2895-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2895-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2895-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c2895-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2895-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2895-108">Prerequisites</span></span>
<span data-ttu-id="c2895-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2895-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2895-111">Permission type</span></span>|<span data-ttu-id="c2895-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2895-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2895-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2895-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2895-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2895-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2895-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2895-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2895-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2895-116">Not supported.</span></span>|
|<span data-ttu-id="c2895-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2895-117">Application</span></span>|<span data-ttu-id="c2895-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2895-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2895-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2895-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="c2895-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2895-120">Request headers</span></span>
|<span data-ttu-id="c2895-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2895-121">Header</span></span>|<span data-ttu-id="c2895-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2895-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2895-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2895-123">Authorization</span></span>|<span data-ttu-id="c2895-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2895-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2895-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2895-125">Accept</span></span>|<span data-ttu-id="c2895-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2895-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2895-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2895-127">Request body</span></span>
<span data-ttu-id="c2895-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2895-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2895-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2895-129">Response</span></span>
<span data-ttu-id="c2895-130">В случае успешной работы эта функция возвращает код отклика и `200 OK` [управлениеConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c2895-130">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2895-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c2895-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2895-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2895-132">Request</span></span>
<span data-ttu-id="c2895-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2895-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="c2895-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2895-134">Response</span></span>
<span data-ttu-id="c2895-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2895-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "value": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  }
}
```




