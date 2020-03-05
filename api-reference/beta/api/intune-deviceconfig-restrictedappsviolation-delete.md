---
title: Удаление Рестриктедаппсвиолатион
description: Удаляет объект Рестриктедаппсвиолатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cc59744e06442aca235ddd166ecdfa97d9cd073
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42483919"
---
# <a name="delete-restrictedappsviolation"></a><span data-ttu-id="e98d3-103">Удаление Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="e98d3-103">Delete restrictedAppsViolation</span></span>

<span data-ttu-id="e98d3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e98d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e98d3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e98d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e98d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e98d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e98d3-107">Удаляет объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="e98d3-107">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e98d3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e98d3-108">Prerequisites</span></span>
<span data-ttu-id="e98d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e98d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e98d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e98d3-111">Permission type</span></span>|<span data-ttu-id="e98d3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e98d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e98d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e98d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e98d3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e98d3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e98d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e98d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e98d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e98d3-116">Not supported.</span></span>|
|<span data-ttu-id="e98d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e98d3-117">Application</span></span>|<span data-ttu-id="e98d3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e98d3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e98d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e98d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="e98d3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e98d3-120">Request headers</span></span>
|<span data-ttu-id="e98d3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e98d3-121">Header</span></span>|<span data-ttu-id="e98d3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e98d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e98d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e98d3-123">Authorization</span></span>|<span data-ttu-id="e98d3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e98d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e98d3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e98d3-125">Accept</span></span>|<span data-ttu-id="e98d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e98d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e98d3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e98d3-127">Request body</span></span>
<span data-ttu-id="e98d3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e98d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e98d3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e98d3-129">Response</span></span>
<span data-ttu-id="e98d3-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e98d3-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e98d3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e98d3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e98d3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e98d3-132">Request</span></span>
<span data-ttu-id="e98d3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e98d3-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="e98d3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e98d3-134">Response</span></span>
<span data-ttu-id="e98d3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e98d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





