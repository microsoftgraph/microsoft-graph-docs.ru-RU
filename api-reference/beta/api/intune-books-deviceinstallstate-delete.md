---
title: Delete deviceInstallState
description: Удаляет объект deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f415b478ff7453a6a1ac7abcdd496ca80f6e4502
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874153"
---
# <a name="delete-deviceinstallstate"></a><span data-ttu-id="f8b55-103">Delete deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="f8b55-103">Delete deviceInstallState</span></span>

> <span data-ttu-id="f8b55-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8b55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b55-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8b55-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8b55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8b55-107">Удаляет объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="f8b55-107">Deletes a [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8b55-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f8b55-108">Prerequisites</span></span>
<span data-ttu-id="f8b55-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8b55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8b55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8b55-111">Permission type</span></span>|<span data-ttu-id="f8b55-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8b55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8b55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8b55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8b55-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b55-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8b55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8b55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8b55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b55-116">Not supported.</span></span>|
|<span data-ttu-id="f8b55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8b55-117">Application</span></span>|<span data-ttu-id="f8b55-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8b55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8b55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f8b55-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8b55-120">Request headers</span></span>
|<span data-ttu-id="f8b55-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8b55-121">Header</span></span>|<span data-ttu-id="f8b55-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8b55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8b55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8b55-123">Authorization</span></span>|<span data-ttu-id="f8b55-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f8b55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8b55-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8b55-125">Accept</span></span>|<span data-ttu-id="f8b55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8b55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8b55-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8b55-127">Request body</span></span>
<span data-ttu-id="f8b55-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8b55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8b55-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8b55-129">Response</span></span>
<span data-ttu-id="f8b55-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8b55-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f8b55-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8b55-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8b55-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8b55-132">Request</span></span>
<span data-ttu-id="f8b55-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8b55-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="f8b55-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8b55-134">Response</span></span>
<span data-ttu-id="f8b55-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f8b55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





