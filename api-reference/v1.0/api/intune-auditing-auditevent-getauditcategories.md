---
title: Функция getAuditCategories
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e85bf6031e881025fe62e902e66add87b0b7c4da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261644"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="1dc88-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="1dc88-103">getAuditCategories function</span></span>

> <span data-ttu-id="1dc88-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dc88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dc88-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1dc88-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dc88-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1dc88-106">Prerequisites</span></span>
<span data-ttu-id="1dc88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1dc88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1dc88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dc88-109">Permission type</span></span>|<span data-ttu-id="1dc88-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dc88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dc88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dc88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1dc88-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dc88-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1dc88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dc88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dc88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dc88-114">Not supported.</span></span>|
|<span data-ttu-id="1dc88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dc88-115">Application</span></span>|<span data-ttu-id="1dc88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dc88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dc88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dc88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="1dc88-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dc88-118">Request headers</span></span>
|<span data-ttu-id="1dc88-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dc88-119">Header</span></span>|<span data-ttu-id="1dc88-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1dc88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dc88-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc88-121">Authorization</span></span>|<span data-ttu-id="1dc88-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1dc88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dc88-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1dc88-123">Accept</span></span>|<span data-ttu-id="1dc88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1dc88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dc88-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dc88-125">Request body</span></span>
<span data-ttu-id="1dc88-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dc88-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dc88-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dc88-127">Response</span></span>
<span data-ttu-id="1dc88-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1dc88-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc88-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1dc88-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dc88-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dc88-130">Request</span></span>
<span data-ttu-id="1dc88-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dc88-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="1dc88-132">Отклик
</span><span class="sxs-lookup"><span data-stu-id="1dc88-132">Response</span></span>
<span data-ttu-id="1dc88-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1dc88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



