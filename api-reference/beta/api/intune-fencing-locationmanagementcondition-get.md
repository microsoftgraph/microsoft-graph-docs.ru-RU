---
title: Получение locationManagementCondition
description: Чтение свойства и связи объекта locationManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65dafbb03b755539bb0a2e919429f3454a225764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953331"
---
# <a name="get-locationmanagementcondition"></a><span data-ttu-id="8c146-103">Получение locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="8c146-103">Get locationManagementCondition</span></span>

> <span data-ttu-id="8c146-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8c146-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c146-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c146-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c146-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c146-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c146-107">Чтение свойства и связи объекта [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="8c146-107">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c146-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8c146-108">Prerequisites</span></span>
<span data-ttu-id="8c146-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c146-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c146-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c146-111">Permission type</span></span>|<span data-ttu-id="8c146-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c146-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c146-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c146-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c146-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c146-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8c146-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c146-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c146-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c146-116">Not supported.</span></span>|
|<span data-ttu-id="8c146-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c146-117">Application</span></span>|<span data-ttu-id="8c146-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c146-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c146-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c146-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c146-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c146-120">Optional query parameters</span></span>
<span data-ttu-id="8c146-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8c146-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8c146-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c146-122">Request headers</span></span>
|<span data-ttu-id="8c146-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c146-123">Header</span></span>|<span data-ttu-id="8c146-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8c146-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c146-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c146-125">Authorization</span></span>|<span data-ttu-id="8c146-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8c146-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c146-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8c146-127">Accept</span></span>|<span data-ttu-id="8c146-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8c146-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c146-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c146-129">Request body</span></span>
<span data-ttu-id="8c146-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c146-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c146-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c146-131">Response</span></span>
<span data-ttu-id="8c146-132">Успешно завершена, этот метод возвращает `200 OK` объект [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8c146-132">If successful, this method returns a `200 OK` response code and [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c146-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8c146-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c146-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c146-134">Request</span></span>
<span data-ttu-id="8c146-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c146-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="8c146-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c146-136">Response</span></span>
<span data-ttu-id="8c146-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8c146-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.locationManagementCondition",
    "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
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





