---
title: Get deviceCompliancePolicy
description: Чтение свойств и связей объекта deviceCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: 54c998f79e8b916e549751186e2967b0482e23bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322794"
---
# <a name="get-devicecompliancepolicy"></a><span data-ttu-id="430db-103">Get deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="430db-103">Get deviceCompliancePolicy</span></span>

> <span data-ttu-id="430db-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="430db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="430db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="430db-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="430db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="430db-107">Чтение свойств и связей объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="430db-107">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="430db-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="430db-108">Prerequisites</span></span>
<span data-ttu-id="430db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="430db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="430db-111">Permission type</span></span>|<span data-ttu-id="430db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="430db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="430db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="430db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="430db-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="430db-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="430db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="430db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="430db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430db-116">Not supported.</span></span>|
|<span data-ttu-id="430db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="430db-117">Application</span></span>|<span data-ttu-id="430db-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="430db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="430db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="430db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="430db-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="430db-120">Optional query parameters</span></span>
<span data-ttu-id="430db-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="430db-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="430db-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="430db-122">Request headers</span></span>
|<span data-ttu-id="430db-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="430db-123">Header</span></span>|<span data-ttu-id="430db-124">Значение</span><span class="sxs-lookup"><span data-stu-id="430db-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="430db-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="430db-125">Authorization</span></span>|<span data-ttu-id="430db-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="430db-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="430db-127">Accept</span><span class="sxs-lookup"><span data-stu-id="430db-127">Accept</span></span>|<span data-ttu-id="430db-128">application/json</span><span class="sxs-lookup"><span data-stu-id="430db-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="430db-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="430db-129">Request body</span></span>
<span data-ttu-id="430db-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="430db-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="430db-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="430db-131">Response</span></span>
<span data-ttu-id="430db-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="430db-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="430db-133">Пример</span><span class="sxs-lookup"><span data-stu-id="430db-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="430db-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="430db-134">Request</span></span>
<span data-ttu-id="430db-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="430db-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="430db-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="430db-136">Response</span></span>
<span data-ttu-id="430db-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="430db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





