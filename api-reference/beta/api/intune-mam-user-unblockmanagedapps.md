---
title: действие Унблоккманажедаппс
description: Разблокирует возврат из приложения для пользователя управляемого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c664f10ac7a3012b13d347cb20b88ee87959850f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011020"
---
# <a name="unblockmanagedapps-action"></a><span data-ttu-id="87371-103">действие Унблоккманажедаппс</span><span class="sxs-lookup"><span data-stu-id="87371-103">unblockManagedApps action</span></span>

<span data-ttu-id="87371-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87371-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87371-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87371-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87371-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87371-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87371-107">Разблокирует возврат из приложения для пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="87371-107">Unblocks the managed app user from app check-in.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87371-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87371-108">Prerequisites</span></span>
<span data-ttu-id="87371-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87371-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87371-111">Permission type</span></span>|<span data-ttu-id="87371-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87371-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87371-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87371-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87371-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87371-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87371-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87371-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87371-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87371-116">Not supported.</span></span>|
|<span data-ttu-id="87371-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87371-117">Application</span></span>|<span data-ttu-id="87371-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87371-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87371-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87371-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/unblockManagedApps
```

## <a name="request-headers"></a><span data-ttu-id="87371-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87371-120">Request headers</span></span>
|<span data-ttu-id="87371-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87371-121">Header</span></span>|<span data-ttu-id="87371-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87371-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87371-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87371-123">Authorization</span></span>|<span data-ttu-id="87371-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87371-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87371-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87371-125">Accept</span></span>|<span data-ttu-id="87371-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87371-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87371-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87371-127">Request body</span></span>
<span data-ttu-id="87371-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87371-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87371-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="87371-129">Response</span></span>
<span data-ttu-id="87371-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="87371-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="87371-131">Пример</span><span class="sxs-lookup"><span data-stu-id="87371-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="87371-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87371-132">Request</span></span>
<span data-ttu-id="87371-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87371-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/unblockManagedApps
```

### <a name="response"></a><span data-ttu-id="87371-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="87371-134">Response</span></span>
<span data-ttu-id="87371-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87371-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






