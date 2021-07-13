---
title: Удаление группы из несовместимых групп
description: Удалите ссылку, которая указывает, что группа несовместима с указанным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9dab2d0aa8278f932648106e2db87eef513aeebd
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401147"
---
# <a name="remove-group-from-incompatiblegroups"></a><span data-ttu-id="93021-103">Удаление группы из несовместимых групп</span><span class="sxs-lookup"><span data-stu-id="93021-103">Remove group from incompatibleGroups</span></span>

<span data-ttu-id="93021-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93021-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93021-105">Удалите [группу](../resources/group.md) из списка групп, которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="93021-105">Remove a [group](../resources/group.md) from the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="93021-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93021-106">Permissions</span></span>

<span data-ttu-id="93021-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93021-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93021-109">Permission type</span></span>                        | <span data-ttu-id="93021-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93021-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93021-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93021-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="93021-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93021-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="93021-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93021-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93021-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93021-114">Not supported.</span></span> |
| <span data-ttu-id="93021-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="93021-115">Application</span></span>                            | <span data-ttu-id="93021-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93021-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93021-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93021-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="93021-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93021-118">Request headers</span></span>

| <span data-ttu-id="93021-119">Имя</span><span class="sxs-lookup"><span data-stu-id="93021-119">Name</span></span>          | <span data-ttu-id="93021-120">Описание</span><span class="sxs-lookup"><span data-stu-id="93021-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="93021-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93021-121">Authorization</span></span> | <span data-ttu-id="93021-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93021-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93021-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93021-124">Content-Type</span></span>  | <span data-ttu-id="93021-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93021-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="93021-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93021-127">Request body</span></span>

<span data-ttu-id="93021-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93021-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93021-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="93021-129">Response</span></span>

<span data-ttu-id="93021-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="93021-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93021-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="93021-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93021-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="93021-133">Request</span></span>

<span data-ttu-id="93021-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93021-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_incompatiblegroup_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```


### <a name="response"></a><span data-ttu-id="93021-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="93021-135">Response</span></span>

<span data-ttu-id="93021-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="93021-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


