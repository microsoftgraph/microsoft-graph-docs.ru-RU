---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e1511b29d9f5369d5eb18e24a5d65e5120322f3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361401"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="fb431-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="fb431-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="fb431-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb431-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb431-105">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="fb431-105">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb431-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fb431-106">Prerequisites</span></span>
<span data-ttu-id="fb431-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb431-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb431-109">Permission type</span></span>|<span data-ttu-id="fb431-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb431-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb431-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb431-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fb431-112">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="fb431-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="fb431-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb431-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb431-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb431-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb431-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb431-115">Not supported.</span></span>|
|<span data-ttu-id="fb431-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb431-116">Application</span></span>|<span data-ttu-id="fb431-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb431-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb431-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb431-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="fb431-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb431-119">Request headers</span></span>
|<span data-ttu-id="fb431-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb431-120">Header</span></span>|<span data-ttu-id="fb431-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fb431-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb431-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb431-122">Authorization</span></span>|<span data-ttu-id="fb431-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb431-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb431-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fb431-124">Accept</span></span>|<span data-ttu-id="fb431-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb431-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb431-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb431-126">Request body</span></span>
<span data-ttu-id="fb431-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb431-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb431-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb431-128">Response</span></span>
<span data-ttu-id="fb431-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb431-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb431-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb431-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb431-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb431-131">Request</span></span>
<span data-ttu-id="fb431-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb431-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="fb431-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb431-133">Response</span></span>
<span data-ttu-id="fb431-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb431-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









