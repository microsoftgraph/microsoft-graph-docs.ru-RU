---
title: Список officeClientConfigurationAssignments
description: Свойства списка и связей объектов officeClientConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 34f926b0e02a963c1ab16ec7a0dd3eefcc06852c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360384"
---
# <a name="list-officeclientconfigurationassignments"></a><span data-ttu-id="329a1-103">Список officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="329a1-103">List officeClientConfigurationAssignments</span></span>

> <span data-ttu-id="329a1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="329a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="329a1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="329a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="329a1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="329a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="329a1-107">Свойства списка и связей объектов [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="329a1-107">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="329a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="329a1-108">Prerequisites</span></span>
<span data-ttu-id="329a1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="329a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="329a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="329a1-111">Permission type</span></span>|<span data-ttu-id="329a1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="329a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="329a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="329a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="329a1-114">\*\* ЗАДАЧ: Определение областей \*\*</span><span class="sxs-lookup"><span data-stu-id="329a1-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="329a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="329a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="329a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="329a1-116">Not supported.</span></span>|
|<span data-ttu-id="329a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="329a1-117">Application</span></span>|<span data-ttu-id="329a1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="329a1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="329a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="329a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="329a1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="329a1-120">Request headers</span></span>
|<span data-ttu-id="329a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="329a1-121">Header</span></span>|<span data-ttu-id="329a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="329a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="329a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="329a1-123">Authorization</span></span>|<span data-ttu-id="329a1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="329a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="329a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="329a1-125">Accept</span></span>|<span data-ttu-id="329a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="329a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="329a1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="329a1-127">Request body</span></span>
<span data-ttu-id="329a1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="329a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="329a1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="329a1-129">Response</span></span>
<span data-ttu-id="329a1-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="329a1-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="329a1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="329a1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="329a1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="329a1-132">Request</span></span>
<span data-ttu-id="329a1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="329a1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="329a1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="329a1-134">Response</span></span>
<span data-ttu-id="329a1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="329a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



