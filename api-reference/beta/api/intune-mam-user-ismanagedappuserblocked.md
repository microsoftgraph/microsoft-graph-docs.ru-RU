---
title: Функция Исманажедаппусерблоккед
description: Получает состояние блокировки пользователя управляемого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0e7249cdc1572524b386c0c4719776dce34666c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708083"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="e1bc0-103">Функция Исманажедаппусерблоккед</span><span class="sxs-lookup"><span data-stu-id="e1bc0-103">isManagedAppUserBlocked function</span></span>

<span data-ttu-id="e1bc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1bc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1bc0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1bc0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1bc0-107">Получает состояние блокировки пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-107">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1bc0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1bc0-108">Prerequisites</span></span>
<span data-ttu-id="e1bc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1bc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1bc0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1bc0-111">Permission type</span></span>|<span data-ttu-id="e1bc0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1bc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1bc0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1bc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1bc0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1bc0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1bc0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1bc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1bc0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-116">Not supported.</span></span>|
|<span data-ttu-id="e1bc0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1bc0-117">Application</span></span>|<span data-ttu-id="e1bc0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1bc0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1bc0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1bc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="e1bc0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1bc0-120">Request headers</span></span>
|<span data-ttu-id="e1bc0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1bc0-121">Header</span></span>|<span data-ttu-id="e1bc0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1bc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1bc0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1bc0-123">Authorization</span></span>|<span data-ttu-id="e1bc0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1bc0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1bc0-125">Accept</span></span>|<span data-ttu-id="e1bc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1bc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1bc0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1bc0-127">Request body</span></span>
<span data-ttu-id="e1bc0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1bc0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1bc0-129">Response</span></span>
<span data-ttu-id="e1bc0-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1bc0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e1bc0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1bc0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1bc0-132">Request</span></span>
<span data-ttu-id="e1bc0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="e1bc0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1bc0-134">Response</span></span>
<span data-ttu-id="e1bc0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1bc0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





