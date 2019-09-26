---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a97610ccd09c7524d0bf9101f53b8ed8f56372d4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194469"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="331b6-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="331b6-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="331b6-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="331b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="331b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="331b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="331b6-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="331b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="331b6-107">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="331b6-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="331b6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="331b6-108">Prerequisites</span></span>
<span data-ttu-id="331b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="331b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="331b6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="331b6-111">Permission type</span></span>|<span data-ttu-id="331b6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="331b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="331b6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="331b6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="331b6-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="331b6-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="331b6-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="331b6-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="331b6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="331b6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="331b6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="331b6-117">Not supported.</span></span>|
|<span data-ttu-id="331b6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="331b6-118">Application</span></span>||
| <span data-ttu-id="331b6-119">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="331b6-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="331b6-120">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="331b6-120">DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="331b6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="331b6-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="331b6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="331b6-122">Request headers</span></span>
|<span data-ttu-id="331b6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="331b6-123">Header</span></span>|<span data-ttu-id="331b6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="331b6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="331b6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="331b6-125">Authorization</span></span>|<span data-ttu-id="331b6-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="331b6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="331b6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="331b6-127">Accept</span></span>|<span data-ttu-id="331b6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="331b6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="331b6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="331b6-129">Request body</span></span>
<span data-ttu-id="331b6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="331b6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="331b6-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="331b6-131">Response</span></span>
<span data-ttu-id="331b6-132">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="331b6-132">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="331b6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="331b6-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="331b6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="331b6-134">Request</span></span>
<span data-ttu-id="331b6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="331b6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="331b6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="331b6-136">Response</span></span>
<span data-ttu-id="331b6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="331b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







