---
title: Удаление accessPackage из несовместимыхAccessPackages
description: Удалите ссылку, которая указывает, что пакет доступа несовместим с указанным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7cb6ad4af6809c75edef5f5e2966eee72a357215
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401151"
---
# <a name="remove-accesspackage-from-incompatibleaccesspackages"></a><span data-ttu-id="00f9b-103">Удаление accessPackage из несовместимыхAccessPackages</span><span class="sxs-lookup"><span data-stu-id="00f9b-103">Remove accessPackage from incompatibleAccessPackages</span></span>

<span data-ttu-id="00f9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00f9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00f9b-105">Удаление пакета [доступа](../resources/accesspackage.md) из списка пакетов доступа, помеченных как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="00f9b-105">Remove an [access package](../resources/accesspackage.md) from the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="00f9b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00f9b-106">Permissions</span></span>

<span data-ttu-id="00f9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00f9b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f9b-109">Permission type</span></span>                        | <span data-ttu-id="00f9b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f9b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="00f9b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f9b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="00f9b-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f9b-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="00f9b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00f9b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f9b-114">Not supported.</span></span> |
| <span data-ttu-id="00f9b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="00f9b-115">Application</span></span>                            | <span data-ttu-id="00f9b-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00f9b-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00f9b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f9b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="00f9b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00f9b-118">Request headers</span></span>

| <span data-ttu-id="00f9b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="00f9b-119">Name</span></span>          | <span data-ttu-id="00f9b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="00f9b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="00f9b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00f9b-121">Authorization</span></span> | <span data-ttu-id="00f9b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f9b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00f9b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00f9b-124">Content-Type</span></span>  | <span data-ttu-id="00f9b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f9b-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00f9b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00f9b-127">Request body</span></span>

<span data-ttu-id="00f9b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00f9b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00f9b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f9b-129">Response</span></span>

<span data-ttu-id="00f9b-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00f9b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00f9b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="00f9b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00f9b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f9b-133">Request</span></span>

<span data-ttu-id="00f9b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00f9b-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_incompatibleaccesspackage_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```


### <a name="response"></a><span data-ttu-id="00f9b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f9b-135">Response</span></span>

<span data-ttu-id="00f9b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="00f9b-136">The following is an example of the response.</span></span>

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
  "description": "Remove incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

