---
title: Функция Исманажедаппусерблоккед
description: Получает состояние блокировки пользователя управляемого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b50a42e4b1994f2efded79d617d5e9484693d55c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011013"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="a2ffd-103">Функция Исманажедаппусерблоккед</span><span class="sxs-lookup"><span data-stu-id="a2ffd-103">isManagedAppUserBlocked function</span></span>

<span data-ttu-id="a2ffd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ffd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ffd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ffd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ffd-107">Получает состояние блокировки пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-107">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2ffd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2ffd-108">Prerequisites</span></span>
<span data-ttu-id="a2ffd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2ffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ffd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2ffd-111">Permission type</span></span>|<span data-ttu-id="a2ffd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2ffd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ffd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2ffd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2ffd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2ffd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a2ffd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2ffd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ffd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-116">Not supported.</span></span>|
|<span data-ttu-id="a2ffd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2ffd-117">Application</span></span>|<span data-ttu-id="a2ffd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2ffd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ffd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2ffd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="a2ffd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2ffd-120">Request headers</span></span>
|<span data-ttu-id="a2ffd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2ffd-121">Header</span></span>|<span data-ttu-id="a2ffd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2ffd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ffd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ffd-123">Authorization</span></span>|<span data-ttu-id="a2ffd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ffd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2ffd-125">Accept</span></span>|<span data-ttu-id="a2ffd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ffd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ffd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2ffd-127">Request body</span></span>
<span data-ttu-id="a2ffd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2ffd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2ffd-129">Response</span></span>
<span data-ttu-id="a2ffd-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ffd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a2ffd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2ffd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2ffd-132">Request</span></span>
<span data-ttu-id="a2ffd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="a2ffd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2ffd-134">Response</span></span>
<span data-ttu-id="a2ffd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2ffd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```






