---
title: действие Жетглобалскрипсигхеставаилаблеверсион
description: Обновление сценария работоспособности собственного устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0bb6f14570ef3a73fe41a6fb2d279e1c77c62bd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162206"
---
# <a name="getglobalscripthighestavailableversion-action"></a><span data-ttu-id="05c85-103">действие Жетглобалскрипсигхеставаилаблеверсион</span><span class="sxs-lookup"><span data-stu-id="05c85-103">getGlobalScriptHighestAvailableVersion action</span></span>

> <span data-ttu-id="05c85-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05c85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05c85-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05c85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c85-106">Обновление сценария работоспособности собственного устройства</span><span class="sxs-lookup"><span data-stu-id="05c85-106">Update the Proprietary Device Health Script</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05c85-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="05c85-107">Prerequisites</span></span>
<span data-ttu-id="05c85-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c85-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05c85-110">Permission type</span></span>|<span data-ttu-id="05c85-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05c85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c85-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05c85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05c85-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05c85-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="05c85-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05c85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05c85-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05c85-115">Not supported.</span></span>|
|<span data-ttu-id="05c85-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05c85-116">Application</span></span>|<span data-ttu-id="05c85-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="05c85-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c85-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05c85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

## <a name="request-headers"></a><span data-ttu-id="05c85-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05c85-119">Request headers</span></span>
|<span data-ttu-id="05c85-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05c85-120">Header</span></span>|<span data-ttu-id="05c85-121">Значение</span><span class="sxs-lookup"><span data-stu-id="05c85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05c85-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05c85-122">Authorization</span></span>|<span data-ttu-id="05c85-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05c85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05c85-124">Accept</span><span class="sxs-lookup"><span data-stu-id="05c85-124">Accept</span></span>|<span data-ttu-id="05c85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05c85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c85-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05c85-126">Request body</span></span>
<span data-ttu-id="05c85-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05c85-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05c85-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="05c85-128">Response</span></span>
<span data-ttu-id="05c85-129">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05c85-129">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c85-130">Пример</span><span class="sxs-lookup"><span data-stu-id="05c85-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="05c85-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="05c85-131">Request</span></span>
<span data-ttu-id="05c85-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05c85-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getGlobalScriptHighestAvailableVersion
```

### <a name="response"></a><span data-ttu-id="05c85-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="05c85-133">Response</span></span>
<span data-ttu-id="05c85-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05c85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 68

{
  "value": "Get Global Script Highest Available Version value"
}
```





