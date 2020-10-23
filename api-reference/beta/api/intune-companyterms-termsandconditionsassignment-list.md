---
title: Перечисление объектов termsAndConditionsAssignment
description: Список свойств и связей объектов termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 090fa1164089260344623377b55fb1927a5bd8c4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731395"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="3814b-103">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="3814b-103">List termsAndConditionsAssignments</span></span>

<span data-ttu-id="3814b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3814b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3814b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3814b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3814b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3814b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3814b-107">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3814b-107">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3814b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3814b-108">Prerequisites</span></span>
<span data-ttu-id="3814b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3814b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3814b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3814b-111">Permission type</span></span>|<span data-ttu-id="3814b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3814b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3814b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3814b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3814b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3814b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3814b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3814b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3814b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3814b-116">Not supported.</span></span>|
|<span data-ttu-id="3814b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3814b-117">Application</span></span>|<span data-ttu-id="3814b-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3814b-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3814b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3814b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3814b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3814b-120">Request headers</span></span>
|<span data-ttu-id="3814b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3814b-121">Header</span></span>|<span data-ttu-id="3814b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3814b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3814b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3814b-123">Authorization</span></span>|<span data-ttu-id="3814b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3814b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3814b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3814b-125">Accept</span></span>|<span data-ttu-id="3814b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3814b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3814b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3814b-127">Request body</span></span>
<span data-ttu-id="3814b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3814b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3814b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3814b-129">Response</span></span>
<span data-ttu-id="3814b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3814b-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3814b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3814b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3814b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3814b-132">Request</span></span>
<span data-ttu-id="3814b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3814b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="3814b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3814b-134">Response</span></span>
<span data-ttu-id="3814b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3814b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```





