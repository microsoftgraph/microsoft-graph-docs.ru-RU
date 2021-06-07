---
title: Delete deviceConfigurationUserStatus
description: Удаляет объект deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f18e94f1d3b0dfc40e7be64283dc511fe8e56528
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752695"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="e2944-103">Delete deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e2944-103">Delete deviceConfigurationUserStatus</span></span>

<span data-ttu-id="e2944-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2944-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2944-106">Удаляет объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e2944-106">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2944-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e2944-107">Prerequisites</span></span>
<span data-ttu-id="e2944-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2944-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2944-110">Permission type</span></span>|<span data-ttu-id="e2944-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2944-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2944-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2944-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2944-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2944-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2944-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2944-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2944-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2944-115">Not supported.</span></span>|
|<span data-ttu-id="e2944-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e2944-116">Application</span></span>|<span data-ttu-id="e2944-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2944-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2944-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2944-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e2944-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2944-119">Request headers</span></span>
|<span data-ttu-id="e2944-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2944-120">Header</span></span>|<span data-ttu-id="e2944-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e2944-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2944-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2944-122">Authorization</span></span>|<span data-ttu-id="e2944-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2944-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2944-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e2944-124">Accept</span></span>|<span data-ttu-id="e2944-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2944-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2944-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2944-126">Request body</span></span>
<span data-ttu-id="e2944-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2944-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2944-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2944-128">Response</span></span>
<span data-ttu-id="e2944-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e2944-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e2944-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e2944-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2944-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2944-131">Request</span></span>
<span data-ttu-id="e2944-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2944-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="e2944-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2944-133">Response</span></span>
<span data-ttu-id="e2944-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2944-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




