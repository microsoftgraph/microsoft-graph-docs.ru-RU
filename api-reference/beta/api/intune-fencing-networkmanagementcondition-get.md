---
title: Получение Нетворкманажементкондитион
description: Чтение свойств и связей объекта Нетворкманажементкондитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9458c87be03494cb124862f9ff9727eea3a0be8e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355355"
---
# <a name="get-networkmanagementcondition"></a><span data-ttu-id="b5633-103">Получение Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="b5633-103">Get networkManagementCondition</span></span>

> <span data-ttu-id="b5633-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5633-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5633-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5633-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5633-106">Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b5633-106">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5633-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5633-107">Prerequisites</span></span>
<span data-ttu-id="b5633-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5633-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5633-110">Permission type</span></span>|<span data-ttu-id="b5633-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5633-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5633-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5633-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5633-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5633-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b5633-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5633-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5633-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5633-115">Not supported.</span></span>|
|<span data-ttu-id="b5633-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5633-116">Application</span></span>|<span data-ttu-id="b5633-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5633-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5633-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5633-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5633-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5633-119">Optional query parameters</span></span>
<span data-ttu-id="b5633-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5633-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5633-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5633-121">Request headers</span></span>
|<span data-ttu-id="b5633-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5633-122">Header</span></span>|<span data-ttu-id="b5633-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b5633-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5633-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5633-124">Authorization</span></span>|<span data-ttu-id="b5633-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5633-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5633-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b5633-126">Accept</span></span>|<span data-ttu-id="b5633-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b5633-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5633-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5633-128">Request body</span></span>
<span data-ttu-id="b5633-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5633-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5633-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5633-130">Response</span></span>
<span data-ttu-id="b5633-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5633-131">If successful, this method returns a `200 OK` response code and [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5633-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b5633-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5633-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5633-133">Request</span></span>
<span data-ttu-id="b5633-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5633-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="b5633-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5633-135">Response</span></span>
<span data-ttu-id="b5633-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5633-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "value": {
    "@odata.type": "#microsoft.graph.networkManagementCondition",
    "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ]
  }
}
```






