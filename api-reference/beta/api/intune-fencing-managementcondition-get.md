---
title: Получение managementCondition
description: Чтение свойства и связи объекта managementCondition.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a6935796d429b478eca53d058690d2e0dcc6ea75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841848"
---
# <a name="get-managementcondition"></a><span data-ttu-id="d33ae-103">Получение managementCondition</span><span class="sxs-lookup"><span data-stu-id="d33ae-103">Get managementCondition</span></span>

> <span data-ttu-id="d33ae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d33ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d33ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d33ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d33ae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d33ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d33ae-107">Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d33ae-107">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d33ae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d33ae-108">Prerequisites</span></span>
<span data-ttu-id="d33ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d33ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d33ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d33ae-111">Permission type</span></span>|<span data-ttu-id="d33ae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d33ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d33ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d33ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d33ae-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d33ae-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d33ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d33ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d33ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d33ae-116">Not supported.</span></span>|
|<span data-ttu-id="d33ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d33ae-117">Application</span></span>|<span data-ttu-id="d33ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d33ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d33ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d33ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d33ae-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d33ae-120">Optional query parameters</span></span>
<span data-ttu-id="d33ae-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d33ae-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d33ae-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d33ae-122">Request headers</span></span>
|<span data-ttu-id="d33ae-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d33ae-123">Header</span></span>|<span data-ttu-id="d33ae-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d33ae-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d33ae-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d33ae-125">Authorization</span></span>|<span data-ttu-id="d33ae-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d33ae-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d33ae-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d33ae-127">Accept</span></span>|<span data-ttu-id="d33ae-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d33ae-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d33ae-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d33ae-129">Request body</span></span>
<span data-ttu-id="d33ae-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d33ae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d33ae-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d33ae-131">Response</span></span>
<span data-ttu-id="d33ae-132">Успешно завершена, этот метод возвращает `200 OK` объект [managementCondition](../resources/intune-fencing-managementcondition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d33ae-132">If successful, this method returns a `200 OK` response code and [managementCondition](../resources/intune-fencing-managementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d33ae-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d33ae-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d33ae-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d33ae-134">Request</span></span>
<span data-ttu-id="d33ae-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d33ae-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="d33ae-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d33ae-136">Response</span></span>
<span data-ttu-id="d33ae-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d33ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 468

{
  "value": {
    "@odata.type": "#microsoft.graph.managementCondition",
    "id": "5cb49381-9381-5cb4-8193-b45c8193b45c",
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





