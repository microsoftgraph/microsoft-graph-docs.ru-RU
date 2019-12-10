---
title: Функция Жетманажеддевицесвисаппфаилурес
description: Получает список устройств с неудачными приложениями
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccea22189a5f47470a0c0f959cdea54e4a077072
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939454"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="b63b3-103">Функция Жетманажеддевицесвисаппфаилурес</span><span class="sxs-lookup"><span data-stu-id="b63b3-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="b63b3-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b63b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b63b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b63b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b63b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b63b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b63b3-107">Получает список устройств с неудачными приложениями</span><span class="sxs-lookup"><span data-stu-id="b63b3-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b63b3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b63b3-108">Prerequisites</span></span>
<span data-ttu-id="b63b3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b63b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b63b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b63b3-111">Permission type</span></span>|<span data-ttu-id="b63b3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b63b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b63b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b63b3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b63b3-114">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b63b3-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b63b3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b63b3-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b63b3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b63b3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b63b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b63b3-117">Not supported.</span></span>|
|<span data-ttu-id="b63b3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b63b3-118">Application</span></span>||
| <span data-ttu-id="b63b3-119">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="b63b3-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b63b3-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b63b3-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b63b3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b63b3-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="b63b3-122">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b63b3-122">Request headers</span></span>
|<span data-ttu-id="b63b3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b63b3-123">Header</span></span>|<span data-ttu-id="b63b3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b63b3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b63b3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b63b3-125">Authorization</span></span>|<span data-ttu-id="b63b3-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b63b3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b63b3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b63b3-127">Accept</span></span>|<span data-ttu-id="b63b3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b63b3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b63b3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b63b3-129">Request body</span></span>
<span data-ttu-id="b63b3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b63b3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b63b3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b63b3-131">Response</span></span>
<span data-ttu-id="b63b3-132">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b63b3-132">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b63b3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b63b3-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b63b3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b63b3-134">Request</span></span>
<span data-ttu-id="b63b3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b63b3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="b63b3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b63b3-136">Response</span></span>
<span data-ttu-id="b63b3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b63b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













