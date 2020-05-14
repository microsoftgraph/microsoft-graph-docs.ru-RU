---
title: Функция getAuditCategories
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7c8b4e9ec640798e01cf2b92ec85a3a2cce5150
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43470509"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="8b527-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="8b527-103">getAuditCategories function</span></span>

<span data-ttu-id="8b527-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b527-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b527-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b527-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b527-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8b527-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b527-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b527-107">Prerequisites</span></span>
<span data-ttu-id="8b527-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b527-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b527-110">Permission type</span></span>|<span data-ttu-id="8b527-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b527-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b527-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b527-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b527-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b527-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8b527-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b527-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b527-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b527-115">Not supported.</span></span>|
|<span data-ttu-id="8b527-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b527-116">Application</span></span>|<span data-ttu-id="8b527-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b527-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b527-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b527-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="8b527-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b527-119">Request headers</span></span>
|<span data-ttu-id="8b527-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b527-120">Header</span></span>|<span data-ttu-id="8b527-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8b527-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b527-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b527-122">Authorization</span></span>|<span data-ttu-id="8b527-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b527-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b527-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8b527-124">Accept</span></span>|<span data-ttu-id="8b527-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b527-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b527-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b527-126">Request body</span></span>
<span data-ttu-id="8b527-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b527-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b527-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b527-128">Response</span></span>
<span data-ttu-id="8b527-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b527-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b527-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8b527-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b527-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b527-131">Request</span></span>
<span data-ttu-id="8b527-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b527-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="8b527-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b527-133">Response</span></span>
<span data-ttu-id="8b527-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b527-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






