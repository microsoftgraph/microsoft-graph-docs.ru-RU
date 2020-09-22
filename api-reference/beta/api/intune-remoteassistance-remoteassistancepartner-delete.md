---
title: Удаление объекта remoteAssistancePartner
description: Удаляет объект remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf9557e2f4487cda07e592b4de827089dfdb4e75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004818"
---
# <a name="delete-remoteassistancepartner"></a><span data-ttu-id="f15fa-103">Удаление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="f15fa-103">Delete remoteAssistancePartner</span></span>

<span data-ttu-id="f15fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f15fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f15fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f15fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f15fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f15fa-107">Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="f15fa-107">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f15fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f15fa-108">Prerequisites</span></span>
<span data-ttu-id="f15fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f15fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f15fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f15fa-111">Permission type</span></span>|<span data-ttu-id="f15fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f15fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f15fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f15fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f15fa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15fa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f15fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f15fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f15fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f15fa-116">Not supported.</span></span>|
|<span data-ttu-id="f15fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f15fa-117">Application</span></span>|<span data-ttu-id="f15fa-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f15fa-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f15fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f15fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="f15fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f15fa-120">Request headers</span></span>
|<span data-ttu-id="f15fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f15fa-121">Header</span></span>|<span data-ttu-id="f15fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f15fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f15fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f15fa-123">Authorization</span></span>|<span data-ttu-id="f15fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f15fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f15fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f15fa-125">Accept</span></span>|<span data-ttu-id="f15fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f15fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f15fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f15fa-127">Request body</span></span>
<span data-ttu-id="f15fa-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f15fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f15fa-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f15fa-129">Response</span></span>
<span data-ttu-id="f15fa-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f15fa-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f15fa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f15fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f15fa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f15fa-132">Request</span></span>
<span data-ttu-id="f15fa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f15fa-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

### <a name="response"></a><span data-ttu-id="f15fa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f15fa-134">Response</span></span>
<span data-ttu-id="f15fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f15fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






