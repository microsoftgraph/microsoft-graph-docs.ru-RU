---
title: Получение locationManagementCondition
description: Чтение свойства и связи объекта locationManagementCondition.
ms.openlocfilehash: df713d68b45c0ad62bce5ade42a53bdc5d69bd83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078430"
---
# <a name="get-locationmanagementcondition"></a><span data-ttu-id="02a23-103">Получение locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="02a23-103">Get locationManagementCondition</span></span>

> <span data-ttu-id="02a23-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02a23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02a23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02a23-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02a23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02a23-107">Чтение свойства и связи объекта [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="02a23-107">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02a23-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02a23-108">Prerequisites</span></span>
<span data-ttu-id="02a23-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02a23-111">Permission type</span></span>|<span data-ttu-id="02a23-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02a23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02a23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02a23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02a23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="02a23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02a23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a23-116">Not supported.</span></span>|
|<span data-ttu-id="02a23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02a23-117">Application</span></span>|<span data-ttu-id="02a23-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a23-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02a23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02a23-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02a23-120">Optional query parameters</span></span>
<span data-ttu-id="02a23-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02a23-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="02a23-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02a23-122">Request headers</span></span>
|<span data-ttu-id="02a23-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02a23-123">Header</span></span>|<span data-ttu-id="02a23-124">Значение</span><span class="sxs-lookup"><span data-stu-id="02a23-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a23-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a23-125">Authorization</span></span>|<span data-ttu-id="02a23-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="02a23-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02a23-127">Accept</span><span class="sxs-lookup"><span data-stu-id="02a23-127">Accept</span></span>|<span data-ttu-id="02a23-128">application/json</span><span class="sxs-lookup"><span data-stu-id="02a23-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a23-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02a23-129">Request body</span></span>
<span data-ttu-id="02a23-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02a23-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02a23-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="02a23-131">Response</span></span>
<span data-ttu-id="02a23-132">Успешно завершена, этот метод возвращает `200 OK` объект [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="02a23-132">If successful, this method returns a `200 OK` response code and [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a23-133">Пример</span><span class="sxs-lookup"><span data-stu-id="02a23-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="02a23-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="02a23-134">Request</span></span>
<span data-ttu-id="02a23-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02a23-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="02a23-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="02a23-136">Response</span></span>
<span data-ttu-id="02a23-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="02a23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





