---
title: Получение Комплианцеманажементпартнер
description: Чтение свойств и связей объекта Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c88d65a85092674bc8790decb2da4bb43a565abc
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744174"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="7e81e-103">Получение Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="7e81e-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="7e81e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e81e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e81e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e81e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e81e-106">Чтение свойств и связей объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="7e81e-106">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e81e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e81e-107">Prerequisites</span></span>
<span data-ttu-id="7e81e-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7e81e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7e81e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e81e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e81e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e81e-110">Permission type</span></span>|<span data-ttu-id="7e81e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e81e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e81e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e81e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e81e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e81e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7e81e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e81e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e81e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e81e-115">Not supported.</span></span>|
|<span data-ttu-id="7e81e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e81e-116">Application</span></span>|<span data-ttu-id="7e81e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e81e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e81e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e81e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e81e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7e81e-119">Optional query parameters</span></span>
<span data-ttu-id="7e81e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7e81e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e81e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e81e-121">Request headers</span></span>
|<span data-ttu-id="7e81e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e81e-122">Header</span></span>|<span data-ttu-id="7e81e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7e81e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e81e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e81e-124">Authorization</span></span>|<span data-ttu-id="7e81e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e81e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e81e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7e81e-126">Accept</span></span>|<span data-ttu-id="7e81e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e81e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e81e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e81e-128">Request body</span></span>
<span data-ttu-id="7e81e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e81e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e81e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e81e-130">Response</span></span>
<span data-ttu-id="7e81e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e81e-131">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e81e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7e81e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e81e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e81e-133">Request</span></span>
<span data-ttu-id="7e81e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e81e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="7e81e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e81e-135">Response</span></span>
<span data-ttu-id="7e81e-136">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="7e81e-136">Here is an example of the response.</span></span> <span data-ttu-id="7e81e-137">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="7e81e-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7e81e-138">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7e81e-138">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1114

{
  "value": {
    "@odata.type": "#microsoft.graph.complianceManagementPartner",
    "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "displayName": "Display Name value",
    "macOsOnboarded": true,
    "androidOnboarded": true,
    "iosOnboarded": true,
    "macOsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ],
    "androidEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ],
    "iosEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ]
  }
}
```



