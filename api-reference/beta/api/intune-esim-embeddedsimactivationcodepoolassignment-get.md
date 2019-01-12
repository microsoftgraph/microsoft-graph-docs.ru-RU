---
title: Получение embeddedSIMActivationCodePoolAssignment
description: Чтение свойства и связи объекта embeddedSIMActivationCodePoolAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 53ffedbb846fd7afe7e03a42f4357a85830e2b18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959743"
---
# <a name="get-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="ea038-103">Получение embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="ea038-103">Get embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="ea038-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea038-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea038-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea038-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea038-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea038-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea038-107">Чтение свойства и связи объекта [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ea038-107">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea038-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea038-108">Prerequisites</span></span>
<span data-ttu-id="ea038-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea038-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea038-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea038-111">Permission type</span></span>|<span data-ttu-id="ea038-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea038-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea038-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea038-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea038-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea038-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea038-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea038-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea038-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea038-116">Not supported.</span></span>|
|<span data-ttu-id="ea038-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea038-117">Application</span></span>|<span data-ttu-id="ea038-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea038-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea038-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea038-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea038-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea038-120">Optional query parameters</span></span>
<span data-ttu-id="ea038-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea038-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea038-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea038-122">Request headers</span></span>
|<span data-ttu-id="ea038-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea038-123">Header</span></span>|<span data-ttu-id="ea038-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ea038-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea038-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea038-125">Authorization</span></span>|<span data-ttu-id="ea038-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ea038-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea038-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ea038-127">Accept</span></span>|<span data-ttu-id="ea038-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ea038-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea038-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea038-129">Request body</span></span>
<span data-ttu-id="ea038-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea038-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea038-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea038-131">Response</span></span>
<span data-ttu-id="ea038-132">Успешно завершена, этот метод возвращает `200 OK` объект [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea038-132">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea038-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ea038-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea038-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea038-134">Request</span></span>
<span data-ttu-id="ea038-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea038-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ea038-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea038-136">Response</span></span>
<span data-ttu-id="ea038-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ea038-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
    "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





