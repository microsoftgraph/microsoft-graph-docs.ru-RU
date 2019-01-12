---
title: Удаление circularGeofenceManagementCondition
description: Удаляет circularGeofenceManagementCondition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 00ada62733c392d0379f5c6dc4bb1a361a8d0c5a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963026"
---
# <a name="delete-circulargeofencemanagementcondition"></a><span data-ttu-id="18d84-103">Удаление circularGeofenceManagementCondition</span><span class="sxs-lookup"><span data-stu-id="18d84-103">Delete circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="18d84-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18d84-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18d84-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18d84-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18d84-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18d84-107">Удаляет [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="18d84-107">Deletes a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18d84-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18d84-108">Prerequisites</span></span>
<span data-ttu-id="18d84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18d84-111">Permission type</span></span>|<span data-ttu-id="18d84-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18d84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18d84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18d84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18d84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18d84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18d84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d84-116">Not supported.</span></span>|
|<span data-ttu-id="18d84-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18d84-117">Application</span></span>|<span data-ttu-id="18d84-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18d84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managementConditions/{managementConditionId}
DELETE /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="18d84-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18d84-120">Request headers</span></span>
|<span data-ttu-id="18d84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18d84-121">Header</span></span>|<span data-ttu-id="18d84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18d84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18d84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18d84-123">Authorization</span></span>|<span data-ttu-id="18d84-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="18d84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18d84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18d84-125">Accept</span></span>|<span data-ttu-id="18d84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18d84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18d84-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18d84-127">Request body</span></span>
<span data-ttu-id="18d84-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18d84-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18d84-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="18d84-129">Response</span></span>
<span data-ttu-id="18d84-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="18d84-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18d84-131">Пример</span><span class="sxs-lookup"><span data-stu-id="18d84-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="18d84-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="18d84-132">Request</span></span>
<span data-ttu-id="18d84-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18d84-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="18d84-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="18d84-134">Response</span></span>
<span data-ttu-id="18d84-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18d84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





