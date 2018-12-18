---
title: Получение embeddedSIMActivationCodePoolAssignment
description: Чтение свойства и связи объекта embeddedSIMActivationCodePoolAssignment.
author: tfitzmac
ms.openlocfilehash: 7663b0f5c57359e3fa9f1f0bff1c746914fae49c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321156"
---
# <a name="get-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="e677a-103">Получение embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="e677a-103">Get embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="e677a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e677a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e677a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e677a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e677a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e677a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e677a-107">Чтение свойства и связи объекта [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e677a-107">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e677a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e677a-108">Prerequisites</span></span>
<span data-ttu-id="e677a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e677a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e677a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e677a-111">Permission type</span></span>|<span data-ttu-id="e677a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e677a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e677a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e677a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e677a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e677a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e677a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e677a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e677a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e677a-116">Not supported.</span></span>|
|<span data-ttu-id="e677a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e677a-117">Application</span></span>|<span data-ttu-id="e677a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e677a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e677a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e677a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e677a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e677a-120">Optional query parameters</span></span>
<span data-ttu-id="e677a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e677a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e677a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e677a-122">Request headers</span></span>
|<span data-ttu-id="e677a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e677a-123">Header</span></span>|<span data-ttu-id="e677a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e677a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e677a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e677a-125">Authorization</span></span>|<span data-ttu-id="e677a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e677a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e677a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e677a-127">Accept</span></span>|<span data-ttu-id="e677a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e677a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e677a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e677a-129">Request body</span></span>
<span data-ttu-id="e677a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e677a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e677a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e677a-131">Response</span></span>
<span data-ttu-id="e677a-132">Успешно завершена, этот метод возвращает `200 OK` объект [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e677a-132">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e677a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e677a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e677a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e677a-134">Request</span></span>
<span data-ttu-id="e677a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e677a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e677a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e677a-136">Response</span></span>
<span data-ttu-id="e677a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e677a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





