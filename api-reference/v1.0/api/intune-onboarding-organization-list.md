---
title: Список организаций
description: Список свойств и связей объектов organization.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 092e8636769b7f1e663ec224609226fc6147de31
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756907"
---
# <a name="list-organizations"></a><span data-ttu-id="4dc62-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="4dc62-103">List organizations</span></span>

<span data-ttu-id="4dc62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dc62-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dc62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc62-106">Список свойств и связей объектов [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="4dc62-106">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dc62-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4dc62-107">Prerequisites</span></span>
<span data-ttu-id="4dc62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc62-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dc62-110">Permission type</span></span>|<span data-ttu-id="4dc62-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dc62-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dc62-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dc62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dc62-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc62-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4dc62-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dc62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dc62-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dc62-115">Not supported.</span></span>|
|<span data-ttu-id="4dc62-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4dc62-116">Application</span></span>|<span data-ttu-id="4dc62-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dc62-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dc62-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dc62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="4dc62-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4dc62-119">Request headers</span></span>
|<span data-ttu-id="4dc62-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dc62-120">Header</span></span>|<span data-ttu-id="4dc62-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4dc62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dc62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dc62-122">Authorization</span></span>|<span data-ttu-id="4dc62-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dc62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dc62-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4dc62-124">Accept</span></span>|<span data-ttu-id="4dc62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dc62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc62-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dc62-126">Request body</span></span>
<span data-ttu-id="4dc62-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dc62-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dc62-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc62-128">Response</span></span>
<span data-ttu-id="4dc62-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4dc62-129">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune-onboarding-organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc62-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4dc62-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dc62-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dc62-131">Request</span></span>
<span data-ttu-id="4dc62-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dc62-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="4dc62-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dc62-133">Response</span></span>
<span data-ttu-id="4dc62-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4dc62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```




