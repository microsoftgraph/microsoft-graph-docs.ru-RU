---
title: функция isManagedAppUserBlocked
description: Получает заблокированную состояние пользователя управляемого приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 07f7295a3096c5c3dd11c6f4903d51b14d67aeb2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148948"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="aebfe-103">функция isManagedAppUserBlocked</span><span class="sxs-lookup"><span data-stu-id="aebfe-103">isManagedAppUserBlocked function</span></span>

<span data-ttu-id="aebfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aebfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aebfe-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aebfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aebfe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aebfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aebfe-107">Получает заблокированную состояние пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="aebfe-107">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aebfe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aebfe-108">Prerequisites</span></span>
<span data-ttu-id="aebfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aebfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aebfe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aebfe-111">Permission type</span></span>|<span data-ttu-id="aebfe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aebfe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aebfe-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aebfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aebfe-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebfe-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aebfe-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aebfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aebfe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aebfe-116">Not supported.</span></span>|
|<span data-ttu-id="aebfe-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aebfe-117">Application</span></span>|<span data-ttu-id="aebfe-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebfe-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aebfe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aebfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="aebfe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aebfe-120">Request headers</span></span>
|<span data-ttu-id="aebfe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aebfe-121">Header</span></span>|<span data-ttu-id="aebfe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aebfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aebfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aebfe-123">Authorization</span></span>|<span data-ttu-id="aebfe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aebfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aebfe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aebfe-125">Accept</span></span>|<span data-ttu-id="aebfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aebfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aebfe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aebfe-127">Request body</span></span>
<span data-ttu-id="aebfe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aebfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aebfe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aebfe-129">Response</span></span>
<span data-ttu-id="aebfe-130">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект Boolean в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aebfe-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aebfe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aebfe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="aebfe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aebfe-132">Request</span></span>
<span data-ttu-id="aebfe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aebfe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="aebfe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aebfe-134">Response</span></span>
<span data-ttu-id="aebfe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aebfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




