---
title: Действие disconnect
description: Запрос на удаление активного соединителя TeamViewer Connector
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2a277d25a9adbf66a8d3b5e0e4e10c9101158c6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698360"
---
# <a name="disconnect-action"></a><span data-ttu-id="c8e87-103">Действие disconnect</span><span class="sxs-lookup"><span data-stu-id="c8e87-103">disconnect action</span></span>

<span data-ttu-id="c8e87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8e87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8e87-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8e87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8e87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8e87-107">Запрос на удаление активного соединителя TeamViewer Connector</span><span class="sxs-lookup"><span data-stu-id="c8e87-107">A request to remove the active TeamViewer connector</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8e87-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8e87-108">Prerequisites</span></span>
<span data-ttu-id="c8e87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e87-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e87-111">Permission type</span></span>|<span data-ttu-id="c8e87-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8e87-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8e87-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e87-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c8e87-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8e87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e87-116">Not supported.</span></span>|
|<span data-ttu-id="c8e87-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8e87-117">Application</span></span>|<span data-ttu-id="c8e87-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e87-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8e87-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

## <a name="request-headers"></a><span data-ttu-id="c8e87-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8e87-120">Request headers</span></span>
|<span data-ttu-id="c8e87-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8e87-121">Header</span></span>|<span data-ttu-id="c8e87-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8e87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8e87-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e87-123">Authorization</span></span>|<span data-ttu-id="c8e87-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8e87-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8e87-125">Accept</span></span>|<span data-ttu-id="c8e87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8e87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e87-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c8e87-127">Request body</span></span>
<span data-ttu-id="c8e87-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8e87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8e87-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e87-129">Response</span></span>
<span data-ttu-id="c8e87-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8e87-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8e87-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c8e87-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8e87-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e87-132">Request</span></span>
<span data-ttu-id="c8e87-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e87-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

### <a name="response"></a><span data-ttu-id="c8e87-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e87-134">Response</span></span>
<span data-ttu-id="c8e87-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8e87-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





