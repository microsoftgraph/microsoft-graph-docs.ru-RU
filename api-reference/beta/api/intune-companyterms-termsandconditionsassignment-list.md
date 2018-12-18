---
title: Перечисление объектов termsAndConditionsAssignment
description: Список свойств и связей объектов termsAndConditionsAssignment.
author: tfitzmac
ms.openlocfilehash: 8f32698a82447e18b6086f565e0acf2f07055662
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340238"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="e40b4-103">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="e40b4-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="e40b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e40b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e40b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e40b4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e40b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e40b4-107">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e40b4-107">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e40b4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e40b4-108">Prerequisites</span></span>
<span data-ttu-id="e40b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e40b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e40b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e40b4-111">Permission type</span></span>|<span data-ttu-id="e40b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e40b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e40b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e40b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e40b4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e40b4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e40b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e40b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e40b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40b4-116">Not supported.</span></span>|
|<span data-ttu-id="e40b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e40b4-117">Application</span></span>|<span data-ttu-id="e40b4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e40b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e40b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e40b4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e40b4-120">Request headers</span></span>
|<span data-ttu-id="e40b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e40b4-121">Header</span></span>|<span data-ttu-id="e40b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e40b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e40b4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e40b4-123">Authorization</span></span>|<span data-ttu-id="e40b4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e40b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e40b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e40b4-125">Accept</span></span>|<span data-ttu-id="e40b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e40b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e40b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e40b4-127">Request body</span></span>
<span data-ttu-id="e40b4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e40b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e40b4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e40b4-129">Response</span></span>
<span data-ttu-id="e40b4-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e40b4-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e40b4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e40b4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e40b4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e40b4-132">Request</span></span>
<span data-ttu-id="e40b4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e40b4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="e40b4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e40b4-134">Response</span></span>
<span data-ttu-id="e40b4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e40b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





