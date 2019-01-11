---
title: Delete windows10GeneralConfiguration
description: Удаляет объект windows10GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fd39ad386ce47973b049ae14f59e53bc82c17b33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852278"
---
# <a name="delete-windows10generalconfiguration"></a><span data-ttu-id="afac7-103">Delete windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="afac7-103">Delete windows10GeneralConfiguration</span></span>

> <span data-ttu-id="afac7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="afac7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afac7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afac7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afac7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afac7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afac7-107">Удаляет объект [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="afac7-107">Deletes a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="afac7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="afac7-108">Prerequisites</span></span>
<span data-ttu-id="afac7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afac7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afac7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afac7-111">Permission type</span></span>|<span data-ttu-id="afac7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="afac7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afac7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afac7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afac7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afac7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afac7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afac7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afac7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afac7-116">Not supported.</span></span>|
|<span data-ttu-id="afac7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afac7-117">Application</span></span>|<span data-ttu-id="afac7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afac7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afac7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afac7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="afac7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="afac7-120">Request headers</span></span>
|<span data-ttu-id="afac7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="afac7-121">Header</span></span>|<span data-ttu-id="afac7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="afac7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afac7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afac7-123">Authorization</span></span>|<span data-ttu-id="afac7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="afac7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afac7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="afac7-125">Accept</span></span>|<span data-ttu-id="afac7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afac7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afac7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="afac7-127">Request body</span></span>
<span data-ttu-id="afac7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="afac7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afac7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="afac7-129">Response</span></span>
<span data-ttu-id="afac7-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="afac7-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="afac7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="afac7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="afac7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="afac7-132">Request</span></span>
<span data-ttu-id="afac7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="afac7-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="afac7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="afac7-134">Response</span></span>
<span data-ttu-id="afac7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="afac7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





