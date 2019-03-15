---
title: Get reportRoot
description: Чтение свойств и связей объекта reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 73eec43bbaf31d39e99cdad5e859debc08b08558
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570936"
---
# <a name="get-reportroot"></a><span data-ttu-id="07cd0-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="07cd0-103">Get reportRoot</span></span>

> <span data-ttu-id="07cd0-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07cd0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07cd0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07cd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07cd0-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07cd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07cd0-107">Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="07cd0-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07cd0-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="07cd0-108">Prerequisites</span></span>
<span data-ttu-id="07cd0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07cd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07cd0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07cd0-111">Permission type</span></span>|<span data-ttu-id="07cd0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07cd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07cd0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07cd0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="07cd0-114">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="07cd0-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="07cd0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="07cd0-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="07cd0-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="07cd0-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="07cd0-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="07cd0-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="07cd0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07cd0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07cd0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07cd0-119">Not supported.</span></span>|
|<span data-ttu-id="07cd0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07cd0-120">Application</span></span>|<span data-ttu-id="07cd0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07cd0-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07cd0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07cd0-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07cd0-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07cd0-123">Optional query parameters</span></span>
<span data-ttu-id="07cd0-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07cd0-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="07cd0-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07cd0-125">Request headers</span></span>
|<span data-ttu-id="07cd0-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07cd0-126">Header</span></span>|<span data-ttu-id="07cd0-127">Значение</span><span class="sxs-lookup"><span data-stu-id="07cd0-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07cd0-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07cd0-128">Authorization</span></span>|<span data-ttu-id="07cd0-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07cd0-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07cd0-130">Accept</span><span class="sxs-lookup"><span data-stu-id="07cd0-130">Accept</span></span>|<span data-ttu-id="07cd0-131">application/json</span><span class="sxs-lookup"><span data-stu-id="07cd0-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07cd0-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07cd0-132">Request body</span></span>
<span data-ttu-id="07cd0-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07cd0-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07cd0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="07cd0-134">Response</span></span>
<span data-ttu-id="07cd0-135">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [reportRoot](../resources/intune-shared-reportroot.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07cd0-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07cd0-136">Пример</span><span class="sxs-lookup"><span data-stu-id="07cd0-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="07cd0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="07cd0-137">Request</span></span>
<span data-ttu-id="07cd0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07cd0-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="07cd0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="07cd0-139">Response</span></span>
<span data-ttu-id="07cd0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07cd0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



