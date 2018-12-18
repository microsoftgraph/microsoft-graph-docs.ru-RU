---
title: Список termsAndConditionsGroupAssignments
description: Свойства списка и связей объектов termsAndConditionsGroupAssignment.
author: tfitzmac
ms.openlocfilehash: b37a75019e57d1ef4a5fb0a290f8bffba2e19fdc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326812"
---
# <a name="list-termsandconditionsgroupassignments"></a><span data-ttu-id="16a15-103">Список termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="16a15-103">List termsAndConditionsGroupAssignments</span></span>

> <span data-ttu-id="16a15-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16a15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16a15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16a15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16a15-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16a15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16a15-107">Свойства списка и связей объектов [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="16a15-107">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16a15-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16a15-108">Prerequisites</span></span>
<span data-ttu-id="16a15-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16a15-111">Permission type</span></span>|<span data-ttu-id="16a15-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16a15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16a15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16a15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16a15-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a15-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="16a15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16a15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16a15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16a15-116">Not supported.</span></span>|
|<span data-ttu-id="16a15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16a15-117">Application</span></span>|<span data-ttu-id="16a15-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16a15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16a15-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16a15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="16a15-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16a15-120">Request headers</span></span>
|<span data-ttu-id="16a15-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16a15-121">Header</span></span>|<span data-ttu-id="16a15-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16a15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16a15-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16a15-123">Authorization</span></span>|<span data-ttu-id="16a15-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="16a15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16a15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16a15-125">Accept</span></span>|<span data-ttu-id="16a15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16a15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16a15-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16a15-127">Request body</span></span>
<span data-ttu-id="16a15-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16a15-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16a15-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="16a15-129">Response</span></span>
<span data-ttu-id="16a15-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16a15-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16a15-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16a15-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="16a15-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="16a15-132">Request</span></span>
<span data-ttu-id="16a15-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16a15-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="16a15-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="16a15-134">Response</span></span>
<span data-ttu-id="16a15-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16a15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 214

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
      "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```





