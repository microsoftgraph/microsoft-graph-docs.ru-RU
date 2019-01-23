---
title: функция getManagedDevicesWithAppFailures
description: Получает список устройств, при помощи неудачных приложений
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d4f2800a187c62c1c6a894817f2405f88c6356d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396807"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="802e3-103">функция getManagedDevicesWithAppFailures</span><span class="sxs-lookup"><span data-stu-id="802e3-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="802e3-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="802e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="802e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="802e3-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="802e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="802e3-107">Получает список устройств, при помощи неудачных приложений</span><span class="sxs-lookup"><span data-stu-id="802e3-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="802e3-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="802e3-108">Prerequisites</span></span>
<span data-ttu-id="802e3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="802e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="802e3-111">Permission type</span></span>|<span data-ttu-id="802e3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="802e3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="802e3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="802e3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="802e3-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="802e3-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="802e3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="802e3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="802e3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="802e3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="802e3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802e3-117">Not supported.</span></span>|
|<span data-ttu-id="802e3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="802e3-118">Application</span></span>|<span data-ttu-id="802e3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802e3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="802e3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="802e3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="802e3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="802e3-121">Request headers</span></span>
|<span data-ttu-id="802e3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="802e3-122">Header</span></span>|<span data-ttu-id="802e3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="802e3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="802e3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="802e3-124">Authorization</span></span>|<span data-ttu-id="802e3-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="802e3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="802e3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="802e3-126">Accept</span></span>|<span data-ttu-id="802e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="802e3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="802e3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="802e3-128">Request body</span></span>
<span data-ttu-id="802e3-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="802e3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="802e3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="802e3-130">Response</span></span>
<span data-ttu-id="802e3-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="802e3-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802e3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="802e3-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="802e3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="802e3-133">Request</span></span>
<span data-ttu-id="802e3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="802e3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="802e3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="802e3-135">Response</span></span>
<span data-ttu-id="802e3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="802e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 74

{
  "value": [
    "Get Managed Devices With App Failures value"
  ]
}
```





