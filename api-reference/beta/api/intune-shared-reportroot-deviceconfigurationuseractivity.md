---
title: Функция deviceConfigurationUserActivity
description: Метаданные для отчета о действиях пользователей с конфигурацией устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c92de4aeb052d62333e0947f08f755a5e05f4d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166988"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="d4085-103">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="d4085-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="d4085-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d4085-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4085-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4085-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4085-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4085-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4085-107">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="d4085-107">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4085-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d4085-108">Prerequisites</span></span>
<span data-ttu-id="d4085-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4085-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="d4085-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4085-111">Permission type</span></span>|<span data-ttu-id="d4085-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4085-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4085-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4085-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d4085-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="d4085-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d4085-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4085-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d4085-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4085-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4085-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4085-117">Not supported.</span></span>|
|<span data-ttu-id="d4085-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4085-118">Application</span></span>|<span data-ttu-id="d4085-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4085-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4085-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4085-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="d4085-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4085-121">Request headers</span></span>
|<span data-ttu-id="d4085-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4085-122">Header</span></span>|<span data-ttu-id="d4085-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d4085-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4085-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4085-124">Authorization</span></span>|<span data-ttu-id="d4085-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d4085-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4085-126">Accept</span><span class="sxs-lookup"><span data-stu-id="d4085-126">Accept</span></span>|<span data-ttu-id="d4085-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d4085-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4085-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4085-128">Request body</span></span>
<span data-ttu-id="d4085-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4085-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4085-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4085-130">Response</span></span>
<span data-ttu-id="d4085-131">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4085-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4085-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d4085-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4085-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4085-133">Request</span></span>
<span data-ttu-id="d4085-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4085-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="d4085-135">Отклик
</span><span class="sxs-lookup"><span data-stu-id="d4085-135">Response</span></span>
<span data-ttu-id="d4085-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4085-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



