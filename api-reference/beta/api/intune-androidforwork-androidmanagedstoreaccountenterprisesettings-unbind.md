---
title: Действие unbind
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea51f38f87861fcfc0fcd7ff9d298a3d5c2a007c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39927442"
---
# <a name="unbind-action"></a><span data-ttu-id="80ae2-103">Действие unbind</span><span class="sxs-lookup"><span data-stu-id="80ae2-103">unbind action</span></span>

> <span data-ttu-id="80ae2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80ae2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80ae2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80ae2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80ae2-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="80ae2-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80ae2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="80ae2-107">Prerequisites</span></span>
<span data-ttu-id="80ae2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80ae2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ae2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80ae2-110">Permission type</span></span>|<span data-ttu-id="80ae2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80ae2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80ae2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80ae2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80ae2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ae2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80ae2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80ae2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80ae2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80ae2-115">Not supported.</span></span>|
|<span data-ttu-id="80ae2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80ae2-116">Application</span></span>|<span data-ttu-id="80ae2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ae2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80ae2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80ae2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/unbind
```

## <a name="request-headers"></a><span data-ttu-id="80ae2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80ae2-119">Request headers</span></span>
|<span data-ttu-id="80ae2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80ae2-120">Header</span></span>|<span data-ttu-id="80ae2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="80ae2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80ae2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80ae2-122">Authorization</span></span>|<span data-ttu-id="80ae2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80ae2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80ae2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="80ae2-124">Accept</span></span>|<span data-ttu-id="80ae2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80ae2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ae2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80ae2-126">Request body</span></span>
<span data-ttu-id="80ae2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80ae2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80ae2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="80ae2-128">Response</span></span>
<span data-ttu-id="80ae2-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80ae2-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80ae2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="80ae2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="80ae2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="80ae2-131">Request</span></span>
<span data-ttu-id="80ae2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80ae2-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/unbind
```

### <a name="response"></a><span data-ttu-id="80ae2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="80ae2-133">Response</span></span>
<span data-ttu-id="80ae2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80ae2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





