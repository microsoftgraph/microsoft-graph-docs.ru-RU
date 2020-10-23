---
title: Получение Манажементкондитионстатемент
description: Чтение свойств и связей объекта Манажементкондитионстатемент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da25211a67d0c1ce00fee7930f832832cdf0d1cc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709445"
---
# <a name="get-managementconditionstatement"></a><span data-ttu-id="4e7be-103">Получение Манажементкондитионстатемент</span><span class="sxs-lookup"><span data-stu-id="4e7be-103">Get managementConditionStatement</span></span>

<span data-ttu-id="4e7be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e7be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e7be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e7be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e7be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e7be-107">Чтение свойств и связей объекта [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) .</span><span class="sxs-lookup"><span data-stu-id="4e7be-107">Read properties and relationships of the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e7be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e7be-108">Prerequisites</span></span>
<span data-ttu-id="4e7be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e7be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e7be-111">Permission type</span></span>|<span data-ttu-id="4e7be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e7be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e7be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e7be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e7be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4e7be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e7be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e7be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e7be-116">Not supported.</span></span>|
|<span data-ttu-id="4e7be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e7be-117">Application</span></span>|<span data-ttu-id="4e7be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e7be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e7be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditionStatements/{managementConditionStatementId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e7be-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e7be-120">Optional query parameters</span></span>
<span data-ttu-id="4e7be-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e7be-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e7be-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e7be-122">Request headers</span></span>
|<span data-ttu-id="4e7be-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e7be-123">Header</span></span>|<span data-ttu-id="4e7be-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4e7be-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e7be-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e7be-125">Authorization</span></span>|<span data-ttu-id="4e7be-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e7be-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e7be-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4e7be-127">Accept</span></span>|<span data-ttu-id="4e7be-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4e7be-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7be-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e7be-129">Request body</span></span>
<span data-ttu-id="4e7be-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e7be-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7be-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e7be-131">Response</span></span>
<span data-ttu-id="4e7be-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e7be-132">If successful, this method returns a `200 OK` response code and [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e7be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4e7be-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e7be-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e7be-134">Request</span></span>
<span data-ttu-id="4e7be-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e7be-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
```

### <a name="response"></a><span data-ttu-id="4e7be-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e7be-136">Response</span></span>
<span data-ttu-id="4e7be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e7be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





