---
title: Список Комплианцеманажементпартнерс
description: Список свойств и связей объектов Комплианцеманажементпартнер.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d36686333ddcd1cb5cf357154a542a67e56718b7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803058"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="eeab5-103">Список Комплианцеманажементпартнерс</span><span class="sxs-lookup"><span data-stu-id="eeab5-103">List complianceManagementPartners</span></span>

> <span data-ttu-id="eeab5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeab5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeab5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eeab5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeab5-106">Список свойств и связей объектов [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) .</span><span class="sxs-lookup"><span data-stu-id="eeab5-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eeab5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eeab5-107">Prerequisites</span></span>
<span data-ttu-id="eeab5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeab5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeab5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeab5-110">Permission type</span></span>|<span data-ttu-id="eeab5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeab5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeab5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeab5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eeab5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeab5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="eeab5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeab5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeab5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeab5-115">Not supported.</span></span>|
|<span data-ttu-id="eeab5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="eeab5-116">Application</span></span>|<span data-ttu-id="eeab5-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeab5-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeab5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeab5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="eeab5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eeab5-119">Request headers</span></span>
|<span data-ttu-id="eeab5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eeab5-120">Header</span></span>|<span data-ttu-id="eeab5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eeab5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeab5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeab5-122">Authorization</span></span>|<span data-ttu-id="eeab5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeab5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeab5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eeab5-124">Accept</span></span>|<span data-ttu-id="eeab5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eeab5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeab5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eeab5-126">Request body</span></span>
<span data-ttu-id="eeab5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eeab5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeab5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="eeab5-128">Response</span></span>
<span data-ttu-id="eeab5-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [комплианцеманажементпартнер](../resources/intune-onboarding-compliancemanagementpartner.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eeab5-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeab5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="eeab5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eeab5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeab5-131">Request</span></span>
<span data-ttu-id="eeab5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeab5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="eeab5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeab5-133">Response</span></span>
<span data-ttu-id="eeab5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eeab5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1490

{
  "value": [
    {
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
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
          }
        }
      ],
      "windowsEnrollmentAssignments": [
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
  ]
}
```




