---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: tfitzmac
ms.openlocfilehash: f19f067212ee6162e2ede9afd325cd80e00af977
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357045"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="52f5f-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="52f5f-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="52f5f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="52f5f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52f5f-105">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="52f5f-105">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52f5f-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="52f5f-106">Prerequisites</span></span>
<span data-ttu-id="52f5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52f5f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52f5f-109">Permission type</span></span>|<span data-ttu-id="52f5f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52f5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52f5f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52f5f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="52f5f-112">&nbsp;&nbsp; Конфигурация устройств</span><span class="sxs-lookup"><span data-stu-id="52f5f-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="52f5f-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52f5f-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52f5f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52f5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52f5f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f5f-115">Not supported.</span></span>|
|<span data-ttu-id="52f5f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52f5f-116">Application</span></span>|<span data-ttu-id="52f5f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52f5f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52f5f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52f5f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="52f5f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52f5f-119">Request headers</span></span>
|<span data-ttu-id="52f5f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52f5f-120">Header</span></span>|<span data-ttu-id="52f5f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="52f5f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52f5f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52f5f-122">Authorization</span></span>|<span data-ttu-id="52f5f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="52f5f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52f5f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="52f5f-124">Accept</span></span>|<span data-ttu-id="52f5f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52f5f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52f5f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52f5f-126">Request body</span></span>
<span data-ttu-id="52f5f-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52f5f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52f5f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="52f5f-128">Response</span></span>
<span data-ttu-id="52f5f-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52f5f-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52f5f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="52f5f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="52f5f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="52f5f-131">Request</span></span>
<span data-ttu-id="52f5f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52f5f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="52f5f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="52f5f-133">Response</span></span>
<span data-ttu-id="52f5f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="52f5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








