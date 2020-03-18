---
title: Функция Жетманажементкондитионстатементекспрессионстринг
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ea31fd0d8d70d2d6258c788b159af84e89f8de9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804753"
---
# <a name="getmanagementconditionstatementexpressionstring-function"></a><span data-ttu-id="b2170-103">Функция Жетманажементкондитионстатементекспрессионстринг</span><span class="sxs-lookup"><span data-stu-id="b2170-103">getManagementConditionStatementExpressionString function</span></span>

> <span data-ttu-id="b2170-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2170-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2170-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2170-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2170-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b2170-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2170-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2170-107">Prerequisites</span></span>
<span data-ttu-id="b2170-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2170-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2170-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2170-110">Permission type</span></span>|<span data-ttu-id="b2170-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2170-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2170-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2170-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2170-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2170-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b2170-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2170-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2170-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2170-115">Not supported.</span></span>|
|<span data-ttu-id="b2170-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2170-116">Application</span></span>|<span data-ttu-id="b2170-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2170-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2170-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2170-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

## <a name="request-headers"></a><span data-ttu-id="b2170-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2170-119">Request headers</span></span>
|<span data-ttu-id="b2170-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2170-120">Header</span></span>|<span data-ttu-id="b2170-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2170-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2170-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2170-122">Authorization</span></span>|<span data-ttu-id="b2170-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2170-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2170-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2170-124">Accept</span></span>|<span data-ttu-id="b2170-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2170-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2170-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2170-126">Request body</span></span>
<span data-ttu-id="b2170-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2170-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2170-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2170-128">Response</span></span>
<span data-ttu-id="b2170-129">В случае успеха эта функция возвращает код `200 OK` отклика и объект [манажементкондитионекспрессионстринг](../resources/intune-fencing-managementconditionexpressionstring.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2170-129">If successful, this function returns a `200 OK` response code and a [managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2170-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b2170-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2170-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2170-131">Request</span></span>
<span data-ttu-id="b2170-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2170-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}/getManagementConditionStatementExpressionString
```

### <a name="response"></a><span data-ttu-id="b2170-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2170-133">Response</span></span>
<span data-ttu-id="b2170-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2170-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




