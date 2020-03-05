---
title: Функция getAuditCategories
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5498006c5564237152383e93ed3bad4c480132a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450400"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="d3f93-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="d3f93-103">getAuditCategories function</span></span>

<span data-ttu-id="d3f93-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3f93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3f93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3f93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3f93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3f93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3f93-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3f93-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3f93-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d3f93-108">Prerequisites</span></span>
<span data-ttu-id="d3f93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3f93-111">Permission type</span></span>|<span data-ttu-id="d3f93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3f93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3f93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3f93-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f93-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d3f93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3f93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3f93-116">Not supported.</span></span>|
|<span data-ttu-id="d3f93-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3f93-117">Application</span></span>|<span data-ttu-id="d3f93-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f93-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3f93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="d3f93-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3f93-120">Request headers</span></span>
|<span data-ttu-id="d3f93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3f93-121">Header</span></span>|<span data-ttu-id="d3f93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3f93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3f93-123">Authorization</span></span>|<span data-ttu-id="d3f93-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3f93-125">Accept</span></span>|<span data-ttu-id="d3f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f93-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3f93-127">Request body</span></span>
<span data-ttu-id="d3f93-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3f93-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3f93-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3f93-129">Response</span></span>
<span data-ttu-id="d3f93-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d3f93-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f93-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d3f93-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3f93-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3f93-132">Request</span></span>
<span data-ttu-id="d3f93-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3f93-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="d3f93-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3f93-134">Response</span></span>
<span data-ttu-id="d3f93-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3f93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





