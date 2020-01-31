---
title: действие Унблоккманажедаппс
description: Разблокирует возврат из приложения для пользователя управляемого приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f5738491a39ff41c80468112850824b9a3b1b378
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636492"
---
# <a name="unblockmanagedapps-action"></a><span data-ttu-id="656b1-103">действие Унблоккманажедаппс</span><span class="sxs-lookup"><span data-stu-id="656b1-103">unblockManagedApps action</span></span>

> <span data-ttu-id="656b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="656b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="656b1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="656b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="656b1-106">Разблокирует возврат из приложения для пользователя управляемого приложения.</span><span class="sxs-lookup"><span data-stu-id="656b1-106">Unblocks the managed app user from app check-in.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="656b1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="656b1-107">Prerequisites</span></span>
<span data-ttu-id="656b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="656b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="656b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="656b1-110">Permission type</span></span>|<span data-ttu-id="656b1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="656b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="656b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="656b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="656b1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="656b1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="656b1-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="656b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="656b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="656b1-115">Not supported.</span></span>|
|<span data-ttu-id="656b1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="656b1-116">Application</span></span>|<span data-ttu-id="656b1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="656b1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="656b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="656b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/unblockManagedApps
```

## <a name="request-headers"></a><span data-ttu-id="656b1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="656b1-119">Request headers</span></span>
|<span data-ttu-id="656b1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="656b1-120">Header</span></span>|<span data-ttu-id="656b1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="656b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="656b1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="656b1-122">Authorization</span></span>|<span data-ttu-id="656b1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="656b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="656b1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="656b1-124">Accept</span></span>|<span data-ttu-id="656b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="656b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="656b1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="656b1-126">Request body</span></span>
<span data-ttu-id="656b1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="656b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="656b1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="656b1-128">Response</span></span>
<span data-ttu-id="656b1-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="656b1-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="656b1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="656b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="656b1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="656b1-131">Request</span></span>
<span data-ttu-id="656b1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="656b1-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/unblockManagedApps
```

### <a name="response"></a><span data-ttu-id="656b1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="656b1-133">Response</span></span>
<span data-ttu-id="656b1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="656b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





