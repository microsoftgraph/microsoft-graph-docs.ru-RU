---
title: Действие syncApps
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43b6aabd722b99c8617122a499049b0e7ed5d9b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417919"
---
# <a name="syncapps-action"></a><span data-ttu-id="17532-103">Действие syncApps</span><span class="sxs-lookup"><span data-stu-id="17532-103">syncApps action</span></span>

<span data-ttu-id="17532-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17532-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17532-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17532-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17532-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17532-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17532-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="17532-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17532-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17532-108">Prerequisites</span></span>
<span data-ttu-id="17532-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17532-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17532-111">Permission type</span></span>|<span data-ttu-id="17532-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17532-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17532-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17532-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17532-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17532-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17532-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17532-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17532-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17532-116">Not supported.</span></span>|
|<span data-ttu-id="17532-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="17532-117">Application</span></span>|<span data-ttu-id="17532-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17532-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17532-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17532-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/syncApps
```

## <a name="request-headers"></a><span data-ttu-id="17532-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17532-120">Request headers</span></span>
|<span data-ttu-id="17532-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17532-121">Header</span></span>|<span data-ttu-id="17532-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17532-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17532-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17532-123">Authorization</span></span>|<span data-ttu-id="17532-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17532-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17532-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17532-125">Accept</span></span>|<span data-ttu-id="17532-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17532-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17532-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17532-127">Request body</span></span>
<span data-ttu-id="17532-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17532-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17532-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="17532-129">Response</span></span>
<span data-ttu-id="17532-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="17532-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="17532-131">Пример</span><span class="sxs-lookup"><span data-stu-id="17532-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="17532-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="17532-132">Request</span></span>
<span data-ttu-id="17532-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17532-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/syncApps
```

### <a name="response"></a><span data-ttu-id="17532-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="17532-134">Response</span></span>
<span data-ttu-id="17532-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17532-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



