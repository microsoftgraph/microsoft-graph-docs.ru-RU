---
title: Функция Жетманажементкондитионстатементекспрессионстринг
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9522b9c18b3bdea9690bfeb62fa6b60c511adab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465746"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="afec7-103">Функция Жетманажементкондитионстатементекспрессионстринг</span><span class="sxs-lookup"><span data-stu-id="afec7-103">getManagementConditionStatementExpressionString function</span></span>

<span data-ttu-id="afec7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="afec7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afec7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afec7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afec7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="afec7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afec7-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="afec7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afec7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="afec7-108">Prerequisites</span></span>
<span data-ttu-id="afec7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afec7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afec7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afec7-111">Permission type</span></span>|<span data-ttu-id="afec7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="afec7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afec7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afec7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afec7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="afec7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="afec7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afec7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afec7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afec7-116">Not supported.</span></span>|
|<span data-ttu-id="afec7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afec7-117">Application</span></span>|<span data-ttu-id="afec7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="afec7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afec7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afec7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="afec7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="afec7-120">Request headers</span></span>
|<span data-ttu-id="afec7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="afec7-121">Header</span></span>|<span data-ttu-id="afec7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="afec7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afec7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afec7-123">Authorization</span></span>|<span data-ttu-id="afec7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="afec7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afec7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="afec7-125">Accept</span></span>|<span data-ttu-id="afec7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afec7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afec7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="afec7-127">Request body</span></span>
<span data-ttu-id="afec7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afec7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afec7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="afec7-129">Response</span></span>
<span data-ttu-id="afec7-130">В случае успеха эта функция возвращает код `200 OK` отклика и объект [манажементкондитионекспрессионстринг](../resources/intune-fencing-managementconditionexpressionstring.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="afec7-130">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afec7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="afec7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="afec7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="afec7-132">Request</span></span>
<span data-ttu-id="afec7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afec7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="afec7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="afec7-134">Response</span></span>
<span data-ttu-id="afec7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="afec7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





