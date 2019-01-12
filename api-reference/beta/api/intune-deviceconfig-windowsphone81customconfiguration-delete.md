---
title: Удаление объекта windowsPhone81CustomConfiguration
description: Удаляет объект windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 89604ad5fdc8892b64b155eb0b7d96fad2e1c9bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930889"
---
# <a name="delete-windowsphone81customconfiguration"></a><span data-ttu-id="b9e71-103">Удаление объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9e71-103">Delete windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="b9e71-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9e71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9e71-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9e71-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9e71-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9e71-107">Удаляет объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b9e71-107">Deletes a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9e71-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9e71-108">Prerequisites</span></span>
<span data-ttu-id="b9e71-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9e71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e71-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9e71-111">Permission type</span></span>|<span data-ttu-id="b9e71-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9e71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9e71-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9e71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9e71-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9e71-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9e71-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9e71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9e71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e71-116">Not supported.</span></span>|
|<span data-ttu-id="b9e71-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9e71-117">Application</span></span>|<span data-ttu-id="b9e71-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9e71-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9e71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b9e71-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9e71-120">Request headers</span></span>
|<span data-ttu-id="b9e71-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9e71-121">Header</span></span>|<span data-ttu-id="b9e71-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9e71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9e71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e71-123">Authorization</span></span>|<span data-ttu-id="b9e71-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b9e71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9e71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9e71-125">Accept</span></span>|<span data-ttu-id="b9e71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9e71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e71-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9e71-127">Request body</span></span>
<span data-ttu-id="b9e71-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9e71-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e71-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9e71-129">Response</span></span>
<span data-ttu-id="b9e71-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b9e71-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9e71-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9e71-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9e71-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9e71-132">Request</span></span>
<span data-ttu-id="b9e71-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9e71-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b9e71-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9e71-134">Response</span></span>
<span data-ttu-id="b9e71-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9e71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





