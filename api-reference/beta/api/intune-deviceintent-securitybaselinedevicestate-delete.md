---
title: Удаление Секуритибаселинедевицестате
description: Удаляет объект Секуритибаселинедевицестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4707f195f8ebfa1108a56ca2eeb1e42aa2aabaa8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381099"
---
# <a name="delete-securitybaselinedevicestate"></a><span data-ttu-id="58313-103">Удаление Секуритибаселинедевицестате</span><span class="sxs-lookup"><span data-stu-id="58313-103">Delete securityBaselineDeviceState</span></span>

<span data-ttu-id="58313-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58313-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58313-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58313-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58313-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58313-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58313-107">Удаляет объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="58313-107">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58313-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58313-108">Prerequisites</span></span>
<span data-ttu-id="58313-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58313-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58313-111">Permission type</span></span>|<span data-ttu-id="58313-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58313-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58313-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58313-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58313-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58313-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58313-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58313-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58313-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58313-116">Not supported.</span></span>|
|<span data-ttu-id="58313-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58313-117">Application</span></span>|<span data-ttu-id="58313-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58313-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58313-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58313-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="58313-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="58313-120">Request headers</span></span>
|<span data-ttu-id="58313-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58313-121">Header</span></span>|<span data-ttu-id="58313-122">Значение</span><span class="sxs-lookup"><span data-stu-id="58313-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58313-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58313-123">Authorization</span></span>|<span data-ttu-id="58313-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58313-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58313-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58313-125">Accept</span></span>|<span data-ttu-id="58313-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58313-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58313-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58313-127">Request body</span></span>
<span data-ttu-id="58313-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58313-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58313-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="58313-129">Response</span></span>
<span data-ttu-id="58313-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="58313-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="58313-131">Пример</span><span class="sxs-lookup"><span data-stu-id="58313-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="58313-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="58313-132">Request</span></span>
<span data-ttu-id="58313-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58313-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="58313-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="58313-134">Response</span></span>
<span data-ttu-id="58313-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58313-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



