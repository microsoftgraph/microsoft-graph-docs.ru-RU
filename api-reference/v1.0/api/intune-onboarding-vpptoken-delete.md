---
title: Удалить vppToken
description: Удаляет vppToken.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfabcbf949706a29ba537a3885734c53635e4577
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757963"
---
# <a name="delete-vpptoken"></a><span data-ttu-id="6797e-103">Удалить vppToken</span><span class="sxs-lookup"><span data-stu-id="6797e-103">Delete vppToken</span></span>

<span data-ttu-id="6797e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6797e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6797e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6797e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6797e-106">Удаляет [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="6797e-106">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6797e-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="6797e-107">Prerequisites</span></span>
<span data-ttu-id="6797e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6797e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6797e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6797e-110">Permission type</span></span>|<span data-ttu-id="6797e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6797e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6797e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6797e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6797e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6797e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6797e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6797e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6797e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6797e-115">Not supported.</span></span>|
|<span data-ttu-id="6797e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6797e-116">Application</span></span>|<span data-ttu-id="6797e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6797e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6797e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6797e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="6797e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6797e-119">Request headers</span></span>
|<span data-ttu-id="6797e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6797e-120">Header</span></span>|<span data-ttu-id="6797e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6797e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6797e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6797e-122">Authorization</span></span>|<span data-ttu-id="6797e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6797e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6797e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6797e-124">Accept</span></span>|<span data-ttu-id="6797e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6797e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6797e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6797e-126">Request body</span></span>
<span data-ttu-id="6797e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6797e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6797e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6797e-128">Response</span></span>
<span data-ttu-id="6797e-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6797e-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6797e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6797e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6797e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6797e-131">Request</span></span>
<span data-ttu-id="6797e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6797e-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="6797e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6797e-133">Response</span></span>
<span data-ttu-id="6797e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6797e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




