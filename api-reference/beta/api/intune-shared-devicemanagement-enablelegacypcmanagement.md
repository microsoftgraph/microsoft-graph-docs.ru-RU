---
title: Действие enableLegacyPcManagement
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 469c1c661d2ad6fec98a5225becde26124942cd1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43390303"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="7ca88-103">Действие enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="7ca88-103">enableLegacyPcManagement action</span></span>

<span data-ttu-id="7ca88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ca88-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ca88-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ca88-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca88-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ca88-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ca88-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ca88-108">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7ca88-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ca88-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ca88-109">Prerequisites</span></span>
<span data-ttu-id="7ca88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ca88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ca88-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ca88-112">Permission type</span></span>|<span data-ttu-id="7ca88-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ca88-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ca88-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ca88-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7ca88-115">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="7ca88-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7ca88-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ca88-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ca88-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ca88-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ca88-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca88-118">Not supported.</span></span>|
|<span data-ttu-id="7ca88-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ca88-119">Application</span></span>||
| <span data-ttu-id="7ca88-120">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="7ca88-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7ca88-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ca88-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ca88-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ca88-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="7ca88-123">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7ca88-123">Request headers</span></span>
|<span data-ttu-id="7ca88-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ca88-124">Header</span></span>|<span data-ttu-id="7ca88-125">Значение</span><span class="sxs-lookup"><span data-stu-id="7ca88-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ca88-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ca88-126">Authorization</span></span>|<span data-ttu-id="7ca88-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ca88-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ca88-128">Accept</span><span class="sxs-lookup"><span data-stu-id="7ca88-128">Accept</span></span>|<span data-ttu-id="7ca88-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7ca88-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ca88-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ca88-130">Request body</span></span>
<span data-ttu-id="7ca88-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ca88-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ca88-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ca88-132">Response</span></span>
<span data-ttu-id="7ca88-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7ca88-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7ca88-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7ca88-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ca88-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ca88-135">Request</span></span>
<span data-ttu-id="7ca88-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ca88-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="7ca88-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ca88-137">Response</span></span>
<span data-ttu-id="7ca88-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ca88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











