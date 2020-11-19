---
title: Получение Комплианцеманажементпартнер
description: Чтение свойств и связей объекта Комплианцеманажементпартнер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a37d8be96299982c9f56ae79e3f200b20b665892
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49305794"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="a715e-103">Получение Комплианцеманажементпартнер</span><span class="sxs-lookup"><span data-stu-id="a715e-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="a715e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a715e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a715e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a715e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a715e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a715e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a715e-107">Чтение свойств и связей объекта [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="a715e-107">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a715e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a715e-108">Prerequisites</span></span>
<span data-ttu-id="a715e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a715e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a715e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a715e-111">Permission type</span></span>|<span data-ttu-id="a715e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a715e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a715e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a715e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a715e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a715e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a715e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a715e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a715e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a715e-116">Not supported.</span></span>|
|<span data-ttu-id="a715e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a715e-117">Application</span></span>|<span data-ttu-id="a715e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a715e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a715e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a715e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a715e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a715e-120">Optional query parameters</span></span>
<span data-ttu-id="a715e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a715e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a715e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a715e-122">Request headers</span></span>
|<span data-ttu-id="a715e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a715e-123">Header</span></span>|<span data-ttu-id="a715e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a715e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a715e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a715e-125">Authorization</span></span>|<span data-ttu-id="a715e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a715e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a715e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a715e-127">Accept</span></span>|<span data-ttu-id="a715e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a715e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a715e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a715e-129">Request body</span></span>
<span data-ttu-id="a715e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a715e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a715e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a715e-131">Response</span></span>
<span data-ttu-id="a715e-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a715e-132">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a715e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a715e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a715e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a715e-134">Request</span></span>
<span data-ttu-id="a715e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a715e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="a715e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a715e-136">Response</span></span>
<span data-ttu-id="a715e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a715e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2110

{
  "value": {
    "@odata.type": "#microsoft.graph.complianceManagementPartner",
    "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "displayName": "Display Name value",
    "macOsOnboarded": true,
    "windowsOnboarded": true,
    "androidOnboarded": true,
    "iosOnboarded": true,
    "macOsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ],
    "windowsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ],
    "androidEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ],
    "iosEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ]
  }
}
```




