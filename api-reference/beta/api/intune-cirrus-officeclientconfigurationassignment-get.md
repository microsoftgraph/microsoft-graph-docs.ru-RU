---
title: Получение officeClientConfigurationAssignment
description: Чтение свойства и связи объекта officeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d74d2982c06a11a71825882d4b3c652ed983ccce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817810"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="e40b7-103">Получение officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e40b7-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="e40b7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e40b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e40b7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e40b7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e40b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e40b7-107">Чтение свойства и связи объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e40b7-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e40b7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e40b7-108">Prerequisites</span></span>
<span data-ttu-id="e40b7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e40b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e40b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e40b7-111">Permission type</span></span>|<span data-ttu-id="e40b7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e40b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e40b7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e40b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e40b7-114">\*\* ЗАДАЧ: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="e40b7-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="e40b7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e40b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e40b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40b7-116">Not supported.</span></span>|
|<span data-ttu-id="e40b7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e40b7-117">Application</span></span>|<span data-ttu-id="e40b7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e40b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e40b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e40b7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e40b7-120">Optional query parameters</span></span>
<span data-ttu-id="e40b7-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e40b7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e40b7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e40b7-122">Request headers</span></span>
|<span data-ttu-id="e40b7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e40b7-123">Header</span></span>|<span data-ttu-id="e40b7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e40b7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e40b7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e40b7-125">Authorization</span></span>|<span data-ttu-id="e40b7-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e40b7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e40b7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e40b7-127">Accept</span></span>|<span data-ttu-id="e40b7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e40b7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e40b7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e40b7-129">Request body</span></span>
<span data-ttu-id="e40b7-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e40b7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e40b7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e40b7-131">Response</span></span>
<span data-ttu-id="e40b7-132">Успешно завершена, этот метод возвращает `200 OK` объект [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e40b7-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e40b7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e40b7-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e40b7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e40b7-134">Request</span></span>
<span data-ttu-id="e40b7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e40b7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e40b7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e40b7-136">Response</span></span>
<span data-ttu-id="e40b7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e40b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```



