---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c83c9a6216e678d16af212f6a31648f7dea8a2b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576925"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="ef42c-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="ef42c-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="ef42c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef42c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef42c-105">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="ef42c-105">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef42c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef42c-106">Prerequisites</span></span>
<span data-ttu-id="ef42c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef42c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef42c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef42c-109">Permission type</span></span>|<span data-ttu-id="ef42c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef42c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef42c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef42c-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ef42c-112">&nbsp;&nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="ef42c-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="ef42c-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef42c-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef42c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef42c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef42c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef42c-115">Not supported.</span></span>|
|<span data-ttu-id="ef42c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef42c-116">Application</span></span>|<span data-ttu-id="ef42c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef42c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef42c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef42c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="ef42c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef42c-119">Request headers</span></span>
|<span data-ttu-id="ef42c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef42c-120">Header</span></span>|<span data-ttu-id="ef42c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef42c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef42c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef42c-122">Authorization</span></span>|<span data-ttu-id="ef42c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef42c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef42c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ef42c-124">Accept</span></span>|<span data-ttu-id="ef42c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef42c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef42c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef42c-126">Request body</span></span>
<span data-ttu-id="ef42c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef42c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef42c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef42c-128">Response</span></span>
<span data-ttu-id="ef42c-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef42c-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef42c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ef42c-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef42c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef42c-131">Request</span></span>
<span data-ttu-id="ef42c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef42c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="ef42c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef42c-133">Response</span></span>
<span data-ttu-id="ef42c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef42c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








