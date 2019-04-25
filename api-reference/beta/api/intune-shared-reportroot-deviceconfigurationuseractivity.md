---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 37aefd42e498d2ed24103017bc3d1c232a774f8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527156"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="8c4fa-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="8c4fa-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="8c4fa-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c4fa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c4fa-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c4fa-107">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="8c4fa-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c4fa-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c4fa-108">Prerequisites</span></span>
<span data-ttu-id="8c4fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c4fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c4fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c4fa-111">Permission type</span></span>|<span data-ttu-id="8c4fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c4fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c4fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c4fa-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c4fa-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="8c4fa-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8c4fa-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c4fa-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8c4fa-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c4fa-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c4fa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-117">Not supported.</span></span>|
|<span data-ttu-id="8c4fa-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c4fa-118">Application</span></span>|<span data-ttu-id="8c4fa-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c4fa-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c4fa-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="8c4fa-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c4fa-121">Request headers</span></span>
|<span data-ttu-id="8c4fa-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c4fa-122">Header</span></span>|<span data-ttu-id="8c4fa-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8c4fa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c4fa-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c4fa-124">Authorization</span></span>|<span data-ttu-id="8c4fa-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c4fa-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8c4fa-126">Accept</span></span>|<span data-ttu-id="8c4fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8c4fa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c4fa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c4fa-128">Request body</span></span>
<span data-ttu-id="8c4fa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c4fa-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c4fa-130">Response</span></span>
<span data-ttu-id="8c4fa-131">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c4fa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8c4fa-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c4fa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c4fa-133">Request</span></span>
<span data-ttu-id="8c4fa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="8c4fa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c4fa-135">Response</span></span>
<span data-ttu-id="8c4fa-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c4fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



