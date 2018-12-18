---
title: Перечисление объектов deviceCompliancePolicyAssignment
description: Список свойств и связей объектов deviceCompliancePolicyAssignment.
author: tfitzmac
ms.openlocfilehash: e1979293e28eb71f142f4631b636ae2f44994e80
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359096"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="b991b-103">Перечисление объектов deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b991b-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="b991b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b991b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b991b-105">Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b991b-105">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b991b-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b991b-106">Prerequisites</span></span>
<span data-ttu-id="b991b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b991b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b991b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b991b-109">Permission type</span></span>|<span data-ttu-id="b991b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b991b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b991b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b991b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b991b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b991b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b991b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b991b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b991b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b991b-114">Not supported.</span></span>|
|<span data-ttu-id="b991b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b991b-115">Application</span></span>|<span data-ttu-id="b991b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b991b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b991b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b991b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b991b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b991b-118">Request headers</span></span>
|<span data-ttu-id="b991b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b991b-119">Header</span></span>|<span data-ttu-id="b991b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b991b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b991b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b991b-121">Authorization</span></span>|<span data-ttu-id="b991b-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b991b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b991b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b991b-123">Accept</span></span>|<span data-ttu-id="b991b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b991b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b991b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b991b-125">Request body</span></span>
<span data-ttu-id="b991b-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b991b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b991b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b991b-127">Response</span></span>
<span data-ttu-id="b991b-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b991b-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b991b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b991b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b991b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b991b-130">Request</span></span>
<span data-ttu-id="b991b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b991b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="b991b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b991b-132">Response</span></span>
<span data-ttu-id="b991b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b991b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



