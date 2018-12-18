---
title: Удаление объекта deviceCompliancePolicyAssignment
description: Удаляет объект deviceCompliancePolicyAssignment.
author: tfitzmac
ms.openlocfilehash: 7fc38acb1e8eed0b61694cf9aa63bec296bfdf89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306540"
---
# <a name="delete-devicecompliancepolicyassignment"></a><span data-ttu-id="cb5f8-103">Удаление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cb5f8-103">Delete deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="cb5f8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb5f8-105">Удаляет объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cb5f8-105">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb5f8-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb5f8-106">Prerequisites</span></span>
<span data-ttu-id="cb5f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb5f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb5f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb5f8-109">Permission type</span></span>|<span data-ttu-id="cb5f8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb5f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb5f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb5f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb5f8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb5f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb5f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb5f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-114">Not supported.</span></span>|
|<span data-ttu-id="cb5f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb5f8-115">Application</span></span>|<span data-ttu-id="cb5f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb5f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb5f8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cb5f8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb5f8-118">Request headers</span></span>
|<span data-ttu-id="cb5f8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb5f8-119">Header</span></span>|<span data-ttu-id="cb5f8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cb5f8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb5f8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb5f8-121">Authorization</span></span>|<span data-ttu-id="cb5f8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cb5f8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb5f8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cb5f8-123">Accept</span></span>|<span data-ttu-id="cb5f8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb5f8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb5f8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb5f8-125">Request body</span></span>
<span data-ttu-id="cb5f8-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb5f8-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb5f8-127">Response</span></span>
<span data-ttu-id="cb5f8-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cb5f8-129">Пример</span><span class="sxs-lookup"><span data-stu-id="cb5f8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb5f8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb5f8-130">Request</span></span>
<span data-ttu-id="cb5f8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="cb5f8-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb5f8-132">Response</span></span>
<span data-ttu-id="cb5f8-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cb5f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



