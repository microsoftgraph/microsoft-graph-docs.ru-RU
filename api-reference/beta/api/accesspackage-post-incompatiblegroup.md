---
title: Добавление группы в несовместимые Группы
description: Добавьте ссылку, чтобы указать, что группа несовместима с указанным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2f599d5fc389040f7f711a08dce04c1c54ef5b3a
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401143"
---
# <a name="add-group-to-incompatiblegroups"></a><span data-ttu-id="7395c-103">Добавление группы в несовместимые Группы</span><span class="sxs-lookup"><span data-stu-id="7395c-103">Add group to incompatibleGroups</span></span>

<span data-ttu-id="7395c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7395c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7395c-105">Добавьте [группу](../resources/group.md) в список групп, которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="7395c-105">Add a [group](../resources/group.md) to the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="7395c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7395c-106">Permissions</span></span>

<span data-ttu-id="7395c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7395c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7395c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7395c-109">Permission type</span></span>                        | <span data-ttu-id="7395c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7395c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7395c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7395c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7395c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7395c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7395c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7395c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7395c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7395c-114">Not supported.</span></span> |
| <span data-ttu-id="7395c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7395c-115">Application</span></span>                            | <span data-ttu-id="7395c-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7395c-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7395c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7395c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7395c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7395c-118">Request headers</span></span>

| <span data-ttu-id="7395c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7395c-119">Name</span></span>          | <span data-ttu-id="7395c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7395c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7395c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7395c-121">Authorization</span></span> | <span data-ttu-id="7395c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7395c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7395c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7395c-124">Content-Type</span></span>  | <span data-ttu-id="7395c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7395c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7395c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7395c-127">Request body</span></span>

<span data-ttu-id="7395c-128">В теле запроса поставляем представление JSON структуры с ИД OData URI [группового](../resources/group.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="7395c-128">In the request body, supply a JSON representation of a structure with the OData id of the URI of a [group](../resources/group.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7395c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7395c-129">Response</span></span>

<span data-ttu-id="7395c-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7395c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7395c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7395c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7395c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7395c-133">Request</span></span>

<span data-ttu-id="7395c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7395c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_incompatiblegroup_to_accesspackage"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/$ref
Content-type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/groups/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
}

### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Created
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

