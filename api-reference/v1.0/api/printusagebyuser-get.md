---
title: Get printUsageByUser
description: Извлечение сводки об использовании пользователя за определенный период времени.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 76341cdcb2b96e57f4c7d0454fe45de977311507
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518124"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="a4dcd-103">Get printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="a4dcd-103">Get printUsageByUser</span></span>
<span data-ttu-id="a4dcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4dcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a4dcd-105">Извлечение сводки об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="a4dcd-106">Описание каждой конечной точки см. в [printUsageByUser.](../resources/printUsageByUser.md)</span><span class="sxs-lookup"><span data-stu-id="a4dcd-106">For descriptions of each endpoint, see [printUsageByUser](../resources/printUsageByUser.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4dcd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4dcd-107">Permissions</span></span>
<span data-ttu-id="a4dcd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4dcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a4dcd-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="a4dcd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4dcd-111">Permission type</span></span> | <span data-ttu-id="a4dcd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4dcd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a4dcd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4dcd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a4dcd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4dcd-114">Reports.Read.All</span></span> |
|<span data-ttu-id="a4dcd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4dcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4dcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-116">Not Supported.</span></span>|
|<span data-ttu-id="a4dcd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4dcd-117">Application</span></span>|<span data-ttu-id="a4dcd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4dcd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4dcd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4dcd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4dcd-120">Optional query parameters</span></span>
<span data-ttu-id="a4dcd-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a4dcd-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a4dcd-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4dcd-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4dcd-123">Request headers</span></span>
|<span data-ttu-id="a4dcd-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a4dcd-124">Name</span></span>|<span data-ttu-id="a4dcd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a4dcd-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4dcd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4dcd-126">Authorization</span></span>|<span data-ttu-id="a4dcd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4dcd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4dcd-129">Request body</span></span>
<span data-ttu-id="a4dcd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4dcd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dcd-131">Response</span></span>

<span data-ttu-id="a4dcd-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageByUser](../resources/printusagebyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printusagebyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4dcd-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4dcd-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4dcd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4dcd-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printusagebyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByUser/{id}
```

### <a name="response"></a><span data-ttu-id="a4dcd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dcd-135">Response</span></span>
<span data-ttu-id="a4dcd-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4dcd-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@contoso.com",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

