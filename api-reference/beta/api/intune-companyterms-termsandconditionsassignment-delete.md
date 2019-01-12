---
title: Удаление объекта termsAndConditionsAssignment
description: Удаляет объект termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a548367fd6d37ebe1f58150d53abeb90cf6f6369
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960940"
---
# <a name="delete-termsandconditionsassignment"></a><span data-ttu-id="2406c-103">Удаление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2406c-103">Delete termsAndConditionsAssignment</span></span>

> <span data-ttu-id="2406c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2406c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2406c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2406c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2406c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2406c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2406c-107">Удаляет объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2406c-107">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2406c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2406c-108">Prerequisites</span></span>
<span data-ttu-id="2406c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2406c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2406c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2406c-111">Permission type</span></span>|<span data-ttu-id="2406c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2406c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2406c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2406c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2406c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2406c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2406c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2406c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2406c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2406c-116">Not supported.</span></span>|
|<span data-ttu-id="2406c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2406c-117">Application</span></span>|<span data-ttu-id="2406c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2406c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2406c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2406c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2406c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2406c-120">Request headers</span></span>
|<span data-ttu-id="2406c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2406c-121">Header</span></span>|<span data-ttu-id="2406c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2406c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2406c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2406c-123">Authorization</span></span>|<span data-ttu-id="2406c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2406c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2406c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2406c-125">Accept</span></span>|<span data-ttu-id="2406c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2406c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2406c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2406c-127">Request body</span></span>
<span data-ttu-id="2406c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2406c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2406c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2406c-129">Response</span></span>
<span data-ttu-id="2406c-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2406c-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2406c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2406c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2406c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2406c-132">Request</span></span>
<span data-ttu-id="2406c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2406c-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="2406c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2406c-134">Response</span></span>
<span data-ttu-id="2406c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2406c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





