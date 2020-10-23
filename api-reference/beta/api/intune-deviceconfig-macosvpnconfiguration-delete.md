---
title: Удаление Макосвпнконфигуратион
description: Удаляет объект Макосвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 857778b63531ea26facaed2cd13bf93b63f42109
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709588"
---
# <a name="delete-macosvpnconfiguration"></a><span data-ttu-id="720af-103">Удаление Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="720af-103">Delete macOSVpnConfiguration</span></span>

<span data-ttu-id="720af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="720af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="720af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="720af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="720af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="720af-107">Удаляет объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="720af-107">Deletes a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="720af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="720af-108">Prerequisites</span></span>
<span data-ttu-id="720af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="720af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="720af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="720af-111">Permission type</span></span>|<span data-ttu-id="720af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="720af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="720af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="720af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="720af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="720af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="720af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="720af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="720af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="720af-116">Not supported.</span></span>|
|<span data-ttu-id="720af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="720af-117">Application</span></span>|<span data-ttu-id="720af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="720af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="720af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="720af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="720af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="720af-120">Request headers</span></span>
|<span data-ttu-id="720af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="720af-121">Header</span></span>|<span data-ttu-id="720af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="720af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="720af-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="720af-123">Authorization</span></span>|<span data-ttu-id="720af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="720af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="720af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="720af-125">Accept</span></span>|<span data-ttu-id="720af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="720af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="720af-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="720af-127">Request body</span></span>
<span data-ttu-id="720af-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="720af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="720af-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="720af-129">Response</span></span>
<span data-ttu-id="720af-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="720af-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="720af-131">Пример</span><span class="sxs-lookup"><span data-stu-id="720af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="720af-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="720af-132">Request</span></span>
<span data-ttu-id="720af-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="720af-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="720af-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="720af-134">Response</span></span>
<span data-ttu-id="720af-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="720af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





