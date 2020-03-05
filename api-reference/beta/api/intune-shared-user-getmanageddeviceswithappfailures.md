---
title: Функция Жетманажеддевицесвисаппфаилурес
description: Получает список устройств с неудачными приложениями
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17b56f1af0553255694c444d898ab85447846753
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458030"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="a8e8b-103">Функция Жетманажеддевицесвисаппфаилурес</span><span class="sxs-lookup"><span data-stu-id="a8e8b-103">getManagedDevicesWithAppFailures function</span></span>

<span data-ttu-id="a8e8b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a8e8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8e8b-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8e8b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8e8b-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8e8b-108">Получает список устройств с неудачными приложениями</span><span class="sxs-lookup"><span data-stu-id="a8e8b-108">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8e8b-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a8e8b-109">Prerequisites</span></span>
<span data-ttu-id="a8e8b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8e8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e8b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8e8b-112">Permission type</span></span>|<span data-ttu-id="a8e8b-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8e8b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8e8b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8e8b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a8e8b-115">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="a8e8b-115">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a8e8b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8e8b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a8e8b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8e8b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8e8b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-118">Not supported.</span></span>|
|<span data-ttu-id="a8e8b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8e8b-119">Application</span></span>||
| <span data-ttu-id="a8e8b-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="a8e8b-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a8e8b-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8e8b-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8e8b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8e8b-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="a8e8b-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a8e8b-123">Request headers</span></span>
|<span data-ttu-id="a8e8b-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8e8b-124">Header</span></span>|<span data-ttu-id="a8e8b-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a8e8b-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8e8b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8e8b-126">Authorization</span></span>|<span data-ttu-id="a8e8b-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8e8b-128">Accept</span><span class="sxs-lookup"><span data-stu-id="a8e8b-128">Accept</span></span>|<span data-ttu-id="a8e8b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a8e8b-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8e8b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8e8b-130">Request body</span></span>
<span data-ttu-id="a8e8b-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8e8b-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8e8b-132">Response</span></span>
<span data-ttu-id="a8e8b-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-133">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e8b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a8e8b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8e8b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8e8b-135">Request</span></span>
<span data-ttu-id="a8e8b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="a8e8b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8e8b-137">Response</span></span>
<span data-ttu-id="a8e8b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8e8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













