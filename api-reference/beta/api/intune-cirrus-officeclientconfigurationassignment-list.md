---
title: Список officeClientConfigurationAssignments
description: Свойства списка и связей объектов officeClientConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e0398e5fe9773171ce8ba5d12c456a287185cdf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954423"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="be8ba-103">Список officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="be8ba-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="be8ba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be8ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be8ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be8ba-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be8ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be8ba-107">Свойства списка и связей объектов [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="be8ba-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be8ba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be8ba-108">Prerequisites</span></span>
<span data-ttu-id="be8ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be8ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be8ba-111">Permission type</span></span>|<span data-ttu-id="be8ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be8ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be8ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be8ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be8ba-114">\*\* ЗАДАЧ: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="be8ba-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="be8ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be8ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be8ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be8ba-116">Not supported.</span></span>|
|<span data-ttu-id="be8ba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be8ba-117">Application</span></span>|<span data-ttu-id="be8ba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be8ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be8ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be8ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="be8ba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be8ba-120">Request headers</span></span>
|<span data-ttu-id="be8ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be8ba-121">Header</span></span>|<span data-ttu-id="be8ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be8ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be8ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be8ba-123">Authorization</span></span>|<span data-ttu-id="be8ba-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be8ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be8ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be8ba-125">Accept</span></span>|<span data-ttu-id="be8ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be8ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be8ba-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be8ba-127">Request body</span></span>
<span data-ttu-id="be8ba-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be8ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be8ba-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="be8ba-129">Response</span></span>
<span data-ttu-id="be8ba-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be8ba-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be8ba-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be8ba-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="be8ba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be8ba-132">Request</span></span>
<span data-ttu-id="be8ba-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be8ba-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="be8ba-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="be8ba-134">Response</span></span>
<span data-ttu-id="be8ba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be8ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
      "id": "804730f3-30f3-8047-f330-4780f3304780",
      "target": {
        "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
      }
    }
  ]
}
```



