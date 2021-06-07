---
title: Функция getAuditCategories
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cbd84df96c898daa8586920eac73b9a36813710
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757567"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="04f42-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="04f42-103">getAuditCategories function</span></span>

<span data-ttu-id="04f42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04f42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04f42-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04f42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04f42-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="04f42-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04f42-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04f42-107">Prerequisites</span></span>
<span data-ttu-id="04f42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04f42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04f42-110">Permission type</span></span>|<span data-ttu-id="04f42-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04f42-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04f42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04f42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04f42-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f42-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04f42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04f42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04f42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04f42-115">Not supported.</span></span>|
|<span data-ttu-id="04f42-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="04f42-116">Application</span></span>|<span data-ttu-id="04f42-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f42-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04f42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04f42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="04f42-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04f42-119">Request headers</span></span>
|<span data-ttu-id="04f42-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04f42-120">Header</span></span>|<span data-ttu-id="04f42-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04f42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04f42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f42-122">Authorization</span></span>|<span data-ttu-id="04f42-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04f42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04f42-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04f42-124">Accept</span></span>|<span data-ttu-id="04f42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04f42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04f42-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04f42-126">Request body</span></span>
<span data-ttu-id="04f42-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04f42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04f42-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="04f42-128">Response</span></span>
<span data-ttu-id="04f42-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04f42-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f42-130">Пример</span><span class="sxs-lookup"><span data-stu-id="04f42-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="04f42-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="04f42-131">Request</span></span>
<span data-ttu-id="04f42-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04f42-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="04f42-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="04f42-133">Response</span></span>
<span data-ttu-id="04f42-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04f42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```




