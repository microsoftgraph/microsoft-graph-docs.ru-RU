---
title: Перечисление объектов termsAndConditionsAssignment
description: Список свойств и связей объектов termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bebc9835771782de7eaa2f28305e77643e0a37d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160727"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="2985c-103">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2985c-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="2985c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2985c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2985c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2985c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2985c-106">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2985c-106">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2985c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2985c-107">Prerequisites</span></span>
<span data-ttu-id="2985c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2985c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2985c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2985c-110">Permission type</span></span>|<span data-ttu-id="2985c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2985c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2985c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2985c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2985c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2985c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2985c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2985c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2985c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2985c-115">Not supported.</span></span>|
|<span data-ttu-id="2985c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2985c-116">Application</span></span>|<span data-ttu-id="2985c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2985c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2985c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2985c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2985c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2985c-119">Request headers</span></span>
|<span data-ttu-id="2985c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2985c-120">Header</span></span>|<span data-ttu-id="2985c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2985c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2985c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2985c-122">Authorization</span></span>|<span data-ttu-id="2985c-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2985c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2985c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2985c-124">Accept</span></span>|<span data-ttu-id="2985c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2985c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2985c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2985c-126">Request body</span></span>
<span data-ttu-id="2985c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2985c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2985c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2985c-128">Response</span></span>
<span data-ttu-id="2985c-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2985c-129">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2985c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2985c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2985c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2985c-131">Request</span></span>
<span data-ttu-id="2985c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2985c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="2985c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="2985c-133">Response</span></span>
<span data-ttu-id="2985c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2985c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




