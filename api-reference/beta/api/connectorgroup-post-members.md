---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad5efa59698d4dcf05365c63eb7f69fa2eb095a6
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862929"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="7fe74-103">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="7fe74-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="7fe74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fe74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fe74-105">Добавление [соединителя](../resources/connector.md) в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="7fe74-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="7fe74-106">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7fe74-106">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7fe74-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe74-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe74-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fe74-108">Permission type</span></span>      | <span data-ttu-id="7fe74-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fe74-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fe74-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fe74-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fe74-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7fe74-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7fe74-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fe74-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe74-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe74-113">Not supported.</span></span>    |
|<span data-ttu-id="7fe74-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fe74-114">Application</span></span> | <span data-ttu-id="7fe74-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe74-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7fe74-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fe74-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7fe74-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fe74-117">Request headers</span></span>
| <span data-ttu-id="7fe74-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7fe74-118">Name</span></span>       | <span data-ttu-id="7fe74-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7fe74-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7fe74-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fe74-120">Authorization</span></span>  | <span data-ttu-id="7fe74-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="7fe74-121">Bearer.</span></span> <span data-ttu-id="7fe74-122">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7fe74-122">Required.</span></span>|
| <span data-ttu-id="7fe74-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7fe74-123">Content-type</span></span> | <span data-ttu-id="7fe74-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="7fe74-124">application/json.</span></span> <span data-ttu-id="7fe74-125">Required.</span><span class="sxs-lookup"><span data-stu-id="7fe74-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fe74-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fe74-126">Request body</span></span>
<span data-ttu-id="7fe74-127">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fe74-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7fe74-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe74-128">Response</span></span>

<span data-ttu-id="7fe74-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fe74-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe74-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7fe74-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fe74-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fe74-131">Request</span></span>
<span data-ttu-id="7fe74-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fe74-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
### <a name="response"></a><span data-ttu-id="7fe74-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe74-133">Response</span></span>
<span data-ttu-id="7fe74-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7fe74-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add connector to connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
