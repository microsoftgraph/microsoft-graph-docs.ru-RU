---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
ms.openlocfilehash: 92a82fc79cbf7e19fa408a51e6c38adc9b32734b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025747"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="b0073-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="b0073-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="b0073-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b0073-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0073-105">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="b0073-105">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0073-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0073-106">Prerequisites</span></span>
<span data-ttu-id="b0073-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0073-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0073-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0073-109">Permission type</span></span>|<span data-ttu-id="b0073-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0073-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0073-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0073-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b0073-112">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="b0073-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="b0073-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0073-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0073-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0073-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0073-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0073-115">Not supported.</span></span>|
|<span data-ttu-id="b0073-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0073-116">Application</span></span>|<span data-ttu-id="b0073-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0073-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0073-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0073-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="b0073-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0073-119">Request headers</span></span>
|<span data-ttu-id="b0073-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0073-120">Header</span></span>|<span data-ttu-id="b0073-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0073-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0073-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0073-122">Authorization</span></span>|<span data-ttu-id="b0073-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b0073-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0073-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b0073-124">Accept</span></span>|<span data-ttu-id="b0073-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0073-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0073-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0073-126">Request body</span></span>
<span data-ttu-id="b0073-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0073-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0073-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0073-128">Response</span></span>
<span data-ttu-id="b0073-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0073-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0073-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b0073-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0073-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0073-131">Request</span></span>
<span data-ttu-id="b0073-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0073-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="b0073-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0073-133">Response</span></span>
<span data-ttu-id="b0073-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b0073-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```








