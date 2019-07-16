---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5915ba99b607f3f7e7518be39181eaa89fc3e45c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726119"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="fa41b-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="fa41b-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="fa41b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa41b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa41b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa41b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa41b-106">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="fa41b-106">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa41b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fa41b-107">Prerequisites</span></span>
<span data-ttu-id="fa41b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa41b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa41b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa41b-110">Permission type</span></span>|<span data-ttu-id="fa41b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa41b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa41b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa41b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa41b-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa41b-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa41b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa41b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa41b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa41b-115">Not supported.</span></span>|
|<span data-ttu-id="fa41b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa41b-116">Application</span></span>|<span data-ttu-id="fa41b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa41b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa41b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa41b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="fa41b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa41b-119">Request headers</span></span>
|<span data-ttu-id="fa41b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa41b-120">Header</span></span>|<span data-ttu-id="fa41b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fa41b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa41b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa41b-122">Authorization</span></span>|<span data-ttu-id="fa41b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa41b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa41b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fa41b-124">Accept</span></span>|<span data-ttu-id="fa41b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa41b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa41b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa41b-126">Request body</span></span>
<span data-ttu-id="fa41b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa41b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa41b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa41b-128">Response</span></span>
<span data-ttu-id="fa41b-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект report в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa41b-129">If successful, this function returns a `200 OK` response code and a report in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa41b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fa41b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa41b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa41b-131">Request</span></span>
<span data-ttu-id="fa41b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa41b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="fa41b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa41b-133">Response</span></span>
<span data-ttu-id="fa41b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa41b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





