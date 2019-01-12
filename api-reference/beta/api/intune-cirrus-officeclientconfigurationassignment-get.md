---
title: Получение officeClientConfigurationAssignment
description: Чтение свойства и связи объекта officeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 10bad7093545d872001d79ce31e86fe578d7c659
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991624"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="27666-103">Получение officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="27666-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="27666-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27666-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27666-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27666-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27666-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27666-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27666-107">Чтение свойства и связи объекта [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="27666-107">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27666-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27666-108">Prerequisites</span></span>
<span data-ttu-id="27666-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27666-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27666-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27666-111">Permission type</span></span>|<span data-ttu-id="27666-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27666-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27666-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27666-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27666-114">\*\* ЗАДАЧ: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="27666-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="27666-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27666-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27666-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27666-116">Not supported.</span></span>|
|<span data-ttu-id="27666-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27666-117">Application</span></span>|<span data-ttu-id="27666-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27666-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27666-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27666-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27666-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27666-120">Optional query parameters</span></span>
<span data-ttu-id="27666-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="27666-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="27666-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27666-122">Request headers</span></span>
|<span data-ttu-id="27666-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27666-123">Header</span></span>|<span data-ttu-id="27666-124">Значение</span><span class="sxs-lookup"><span data-stu-id="27666-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27666-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="27666-125">Authorization</span></span>|<span data-ttu-id="27666-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="27666-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27666-127">Accept</span><span class="sxs-lookup"><span data-stu-id="27666-127">Accept</span></span>|<span data-ttu-id="27666-128">application/json</span><span class="sxs-lookup"><span data-stu-id="27666-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27666-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27666-129">Request body</span></span>
<span data-ttu-id="27666-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27666-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27666-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="27666-131">Response</span></span>
<span data-ttu-id="27666-132">Успешно завершена, этот метод возвращает `200 OK` объект [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="27666-132">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27666-133">Пример</span><span class="sxs-lookup"><span data-stu-id="27666-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="27666-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="27666-134">Request</span></span>
<span data-ttu-id="27666-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27666-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="27666-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="27666-136">Response</span></span>
<span data-ttu-id="27666-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="27666-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



