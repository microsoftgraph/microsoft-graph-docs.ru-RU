---
title: Удаление развертывания
description: Удаление объекта развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 305e905c254fc2a5acf66747f147cc009b41ae6a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068197"
---
# <a name="delete-deployment"></a><span data-ttu-id="1569f-103">Удаление развертывания</span><span class="sxs-lookup"><span data-stu-id="1569f-103">Delete deployment</span></span>
<span data-ttu-id="1569f-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="1569f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1569f-105">Удаление [объекта развертывания.](../resources/windowsupdates-deployment.md)</span><span class="sxs-lookup"><span data-stu-id="1569f-105">Delete a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1569f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1569f-106">Permissions</span></span>
<span data-ttu-id="1569f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1569f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1569f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1569f-109">Permission type</span></span>|<span data-ttu-id="1569f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1569f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1569f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1569f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1569f-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1569f-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="1569f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1569f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1569f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1569f-114">Not supported.</span></span>|
|<span data-ttu-id="1569f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1569f-115">Application</span></span>|<span data-ttu-id="1569f-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1569f-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1569f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1569f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="1569f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1569f-118">Request headers</span></span>
|<span data-ttu-id="1569f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1569f-119">Name</span></span>|<span data-ttu-id="1569f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1569f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1569f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1569f-121">Authorization</span></span>|<span data-ttu-id="1569f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1569f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1569f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1569f-124">Request body</span></span>
<span data-ttu-id="1569f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1569f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1569f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1569f-126">Response</span></span>

<span data-ttu-id="1569f-p103">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1569f-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1569f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="1569f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1569f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1569f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_deployment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}
```


### <a name="response"></a><span data-ttu-id="1569f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1569f-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

