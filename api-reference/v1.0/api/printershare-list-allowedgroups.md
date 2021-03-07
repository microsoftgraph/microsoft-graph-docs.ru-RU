---
title: Список разрешенных Групп для принтераShare
description: Извлечение списка групп, которые получили доступ для отправки заданий печати в связанную долю принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a7254feef5bc0c320ab39404c7c7a2f9bc3ccd9c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517433"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="efe05-103">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="efe05-103">List allowedGroups</span></span>
<span data-ttu-id="efe05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="efe05-105">Извлечение списка групп, которые получили доступ для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="efe05-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="efe05-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efe05-106">Permissions</span></span>
<span data-ttu-id="efe05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efe05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="efe05-109">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, да которое предоставляет доступ [к группам](group-list.md) списков.</span><span class="sxs-lookup"><span data-stu-id="efe05-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="efe05-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="efe05-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="efe05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efe05-111">Permission type</span></span> | <span data-ttu-id="efe05-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efe05-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="efe05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efe05-113">Delegated (work or school account)</span></span>| <span data-ttu-id="efe05-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efe05-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="efe05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efe05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efe05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efe05-116">Not Supported.</span></span>|
|<span data-ttu-id="efe05-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="efe05-117">Application</span></span>|<span data-ttu-id="efe05-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efe05-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efe05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efe05-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="efe05-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efe05-120">Request headers</span></span>
|<span data-ttu-id="efe05-121">Имя</span><span class="sxs-lookup"><span data-stu-id="efe05-121">Name</span></span>|<span data-ttu-id="efe05-122">Описание</span><span class="sxs-lookup"><span data-stu-id="efe05-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="efe05-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efe05-123">Authorization</span></span>|<span data-ttu-id="efe05-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efe05-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="efe05-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="efe05-126">Request body</span></span>
<span data-ttu-id="efe05-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efe05-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efe05-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="efe05-128">Response</span></span>

<span data-ttu-id="efe05-129">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="efe05-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efe05-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="efe05-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efe05-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="efe05-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups
```


### <a name="response"></a><span data-ttu-id="efe05-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="efe05-132">Response</span></span>
<span data-ttu-id="efe05-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="efe05-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.group)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

