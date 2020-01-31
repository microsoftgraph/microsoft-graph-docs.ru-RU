---
title: Функция Исманажедаппусерблоккед
description: Получает состояние блокировки пользователя управляемого приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41b4a113dd2aa774df59368dde15f1b0f11aa84a
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636499"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="66dd1-103">Функция Исманажедаппусерблоккед</span><span class="sxs-lookup"><span data-stu-id="66dd1-103">isManagedAppUserBlocked function</span></span>

> <span data-ttu-id="66dd1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66dd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66dd1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66dd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66dd1-106">Получает состояние блокировки пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="66dd1-106">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66dd1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="66dd1-107">Prerequisites</span></span>
<span data-ttu-id="66dd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66dd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66dd1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66dd1-110">Permission type</span></span>|<span data-ttu-id="66dd1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66dd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66dd1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66dd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66dd1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66dd1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="66dd1-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66dd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66dd1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66dd1-115">Not supported.</span></span>|
|<span data-ttu-id="66dd1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66dd1-116">Application</span></span>|<span data-ttu-id="66dd1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66dd1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66dd1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66dd1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="66dd1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66dd1-119">Request headers</span></span>
|<span data-ttu-id="66dd1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66dd1-120">Header</span></span>|<span data-ttu-id="66dd1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="66dd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66dd1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66dd1-122">Authorization</span></span>|<span data-ttu-id="66dd1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66dd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66dd1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="66dd1-124">Accept</span></span>|<span data-ttu-id="66dd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66dd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66dd1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66dd1-126">Request body</span></span>
<span data-ttu-id="66dd1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66dd1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66dd1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="66dd1-128">Response</span></span>
<span data-ttu-id="66dd1-129">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="66dd1-129">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66dd1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="66dd1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="66dd1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="66dd1-131">Request</span></span>
<span data-ttu-id="66dd1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66dd1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="66dd1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="66dd1-133">Response</span></span>
<span data-ttu-id="66dd1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66dd1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





