---
title: Действие assign
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 664265fc65ccf294e7406f23c557a635fad1d384
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358893"
---
# <a name="assign-action"></a><span data-ttu-id="420cf-103">Действие assign</span><span class="sxs-lookup"><span data-stu-id="420cf-103">assign action</span></span>

> <span data-ttu-id="420cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="420cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="420cf-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="420cf-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="420cf-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="420cf-106">Prerequisites</span></span>
<span data-ttu-id="420cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="420cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="420cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="420cf-109">Permission type</span></span>|<span data-ttu-id="420cf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="420cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="420cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="420cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="420cf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="420cf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="420cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="420cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="420cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="420cf-114">Not supported.</span></span>|
|<span data-ttu-id="420cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="420cf-115">Application</span></span>|<span data-ttu-id="420cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="420cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="420cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="420cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="420cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="420cf-118">Request headers</span></span>
|<span data-ttu-id="420cf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="420cf-119">Header</span></span>|<span data-ttu-id="420cf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="420cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="420cf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="420cf-121">Authorization</span></span>|<span data-ttu-id="420cf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="420cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="420cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="420cf-123">Accept</span></span>|<span data-ttu-id="420cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="420cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="420cf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="420cf-125">Request body</span></span>
<span data-ttu-id="420cf-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="420cf-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="420cf-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="420cf-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="420cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="420cf-128">Property</span></span>|<span data-ttu-id="420cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="420cf-129">Type</span></span>|<span data-ttu-id="420cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="420cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="420cf-131">assignments</span><span class="sxs-lookup"><span data-stu-id="420cf-131">assignments</span></span>|<span data-ttu-id="420cf-132">Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="420cf-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="420cf-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="420cf-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="420cf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="420cf-134">Response</span></span>
<span data-ttu-id="420cf-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="420cf-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="420cf-136">Пример</span><span class="sxs-lookup"><span data-stu-id="420cf-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="420cf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="420cf-137">Request</span></span>
<span data-ttu-id="420cf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="420cf-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="420cf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="420cf-139">Response</span></span>
<span data-ttu-id="420cf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="420cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



