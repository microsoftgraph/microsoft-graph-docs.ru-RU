---
title: Удаление Коннектедорганизатион
description: Удаление Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f91652b8f7ec479892c6f19d9804b39b521fe58
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510258"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="25973-103">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="25973-103">Delete connectedOrganization</span></span>

<span data-ttu-id="25973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25973-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25973-105">Удаление объекта [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="25973-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25973-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25973-106">Permissions</span></span>

<span data-ttu-id="25973-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25973-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25973-109">Permission type</span></span>|<span data-ttu-id="25973-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25973-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="25973-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25973-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25973-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25973-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="25973-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25973-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25973-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25973-114">Not supported.</span></span> |
| <span data-ttu-id="25973-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25973-115">Application</span></span>                            | <span data-ttu-id="25973-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25973-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25973-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25973-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="25973-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25973-118">Request headers</span></span>
|<span data-ttu-id="25973-119">Имя</span><span class="sxs-lookup"><span data-stu-id="25973-119">Name</span></span>|<span data-ttu-id="25973-120">Описание</span><span class="sxs-lookup"><span data-stu-id="25973-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="25973-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25973-121">Authorization</span></span>|<span data-ttu-id="25973-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25973-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25973-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25973-124">Request body</span></span>
<span data-ttu-id="25973-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25973-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25973-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="25973-126">Response</span></span>

<span data-ttu-id="25973-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25973-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25973-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="25973-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25973-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="25973-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```


### <a name="response"></a><span data-ttu-id="25973-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="25973-130">Response</span></span>
<span data-ttu-id="25973-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="25973-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
