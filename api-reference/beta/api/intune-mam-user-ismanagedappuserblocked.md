---
title: Функция Исманажедаппусерблоккед
description: Получает состояние блокировки пользователя управляемого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8711b1157ade9dba9e1fa9191e76d5ecd404698e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277381"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="d397e-103">Функция Исманажедаппусерблоккед</span><span class="sxs-lookup"><span data-stu-id="d397e-103">isManagedAppUserBlocked function</span></span>

<span data-ttu-id="d397e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d397e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d397e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d397e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d397e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d397e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d397e-107">Получает состояние блокировки пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="d397e-107">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d397e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d397e-108">Prerequisites</span></span>
<span data-ttu-id="d397e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d397e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d397e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d397e-111">Permission type</span></span>|<span data-ttu-id="d397e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d397e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d397e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d397e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d397e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d397e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d397e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d397e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d397e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d397e-116">Not supported.</span></span>|
|<span data-ttu-id="d397e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d397e-117">Application</span></span>|<span data-ttu-id="d397e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d397e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d397e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d397e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="d397e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d397e-120">Request headers</span></span>
|<span data-ttu-id="d397e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d397e-121">Header</span></span>|<span data-ttu-id="d397e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d397e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d397e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d397e-123">Authorization</span></span>|<span data-ttu-id="d397e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d397e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d397e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d397e-125">Accept</span></span>|<span data-ttu-id="d397e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d397e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d397e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d397e-127">Request body</span></span>
<span data-ttu-id="d397e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d397e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d397e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d397e-129">Response</span></span>
<span data-ttu-id="d397e-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d397e-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d397e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d397e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d397e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d397e-132">Request</span></span>
<span data-ttu-id="d397e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d397e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="d397e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d397e-134">Response</span></span>
<span data-ttu-id="d397e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d397e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




