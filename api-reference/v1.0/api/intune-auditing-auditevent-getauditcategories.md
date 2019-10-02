---
title: Функция getAuditCategories
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4936bbd47b22440e96e27df85002c98c016aeb0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354849"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="3cbc1-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="3cbc1-103">getAuditCategories function</span></span>

> <span data-ttu-id="3cbc1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cbc1-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cbc1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3cbc1-106">Prerequisites</span></span>
<span data-ttu-id="3cbc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cbc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cbc1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cbc1-109">Permission type</span></span>|<span data-ttu-id="3cbc1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cbc1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cbc1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cbc1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cbc1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cbc1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3cbc1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cbc1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cbc1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-114">Not supported.</span></span>|
|<span data-ttu-id="3cbc1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cbc1-115">Application</span></span>|<span data-ttu-id="3cbc1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cbc1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cbc1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="3cbc1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cbc1-118">Request headers</span></span>
|<span data-ttu-id="3cbc1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cbc1-119">Header</span></span>|<span data-ttu-id="3cbc1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3cbc1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cbc1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cbc1-121">Authorization</span></span>|<span data-ttu-id="3cbc1-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cbc1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3cbc1-123">Accept</span></span>|<span data-ttu-id="3cbc1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3cbc1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cbc1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cbc1-125">Request body</span></span>
<span data-ttu-id="3cbc1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cbc1-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cbc1-127">Response</span></span>
<span data-ttu-id="3cbc1-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cbc1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3cbc1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cbc1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cbc1-130">Request</span></span>
<span data-ttu-id="3cbc1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="3cbc1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cbc1-132">Response</span></span>
<span data-ttu-id="3cbc1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cbc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




