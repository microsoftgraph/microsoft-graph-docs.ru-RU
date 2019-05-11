---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d347aacefbe177174115433f1f03b6115101bf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899071"
---
# <a name="get-reportroot"></a><span data-ttu-id="f8751-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="f8751-103">Get reportRoot</span></span>

> <span data-ttu-id="f8751-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8751-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8751-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8751-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8751-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8751-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8751-107">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="f8751-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8751-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f8751-108">Prerequisites</span></span>
<span data-ttu-id="f8751-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8751-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8751-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8751-111">Permission type</span></span>|<span data-ttu-id="f8751-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8751-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8751-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8751-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f8751-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="f8751-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f8751-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8751-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="f8751-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f8751-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f8751-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8751-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f8751-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8751-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8751-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8751-119">Not supported.</span></span>|
|<span data-ttu-id="f8751-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8751-120">Application</span></span>|<span data-ttu-id="f8751-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8751-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8751-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8751-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8751-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f8751-123">Optional query parameters</span></span>
<span data-ttu-id="f8751-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f8751-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8751-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8751-125">Request headers</span></span>
|<span data-ttu-id="f8751-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8751-126">Header</span></span>|<span data-ttu-id="f8751-127">Значение</span><span class="sxs-lookup"><span data-stu-id="f8751-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8751-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8751-128">Authorization</span></span>|<span data-ttu-id="f8751-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8751-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8751-130">Accept</span><span class="sxs-lookup"><span data-stu-id="f8751-130">Accept</span></span>|<span data-ttu-id="f8751-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f8751-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8751-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8751-132">Request body</span></span>
<span data-ttu-id="f8751-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8751-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8751-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8751-134">Response</span></span>
<span data-ttu-id="f8751-135">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f8751-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8751-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f8751-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8751-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8751-137">Request</span></span>
<span data-ttu-id="f8751-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8751-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="f8751-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8751-139">Response</span></span>
<span data-ttu-id="f8751-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8751-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```



