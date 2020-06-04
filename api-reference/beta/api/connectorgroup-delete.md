---
title: Удаление Коннекторграуп
description: Удаление объекта Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45b0216562ce8fefa139726446fbf3eb97daaabd
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556067"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="5c4a1-103">Удаление Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="5c4a1-103">Delete connectorGroup</span></span>

<span data-ttu-id="5c4a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c4a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c4a1-105">Удаление объекта [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="5c4a1-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="5c4a1-106">Все [соединители](../resources/connector.md) и приложения необходимо удалить из группы соединителей, прежде чем можно будет удалить группу соединителей.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c4a1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c4a1-107">Permissions</span></span>
<span data-ttu-id="5c4a1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c4a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5c4a1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c4a1-110">Permission type</span></span>      | <span data-ttu-id="5c4a1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c4a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c4a1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c4a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c4a1-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c4a1-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c4a1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c4a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c4a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-115">Not supported.</span></span>    |
|<span data-ttu-id="5c4a1-116">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="5c4a1-116">Application</span></span> | <span data-ttu-id="5c4a1-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c4a1-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c4a1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c4a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5c4a1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c4a1-119">Request headers</span></span>
| <span data-ttu-id="5c4a1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5c4a1-120">Name</span></span>       | <span data-ttu-id="5c4a1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5c4a1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5c4a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c4a1-122">Authorization</span></span>  | <span data-ttu-id="5c4a1-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-123">Bearer.</span></span> <span data-ttu-id="5c4a1-124">Обязательное</span><span class="sxs-lookup"><span data-stu-id="5c4a1-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c4a1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c4a1-125">Request body</span></span>
<span data-ttu-id="5c4a1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c4a1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c4a1-127">Response</span></span>

<span data-ttu-id="5c4a1-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c4a1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5c4a1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c4a1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c4a1-131">Request</span></span>
<span data-ttu-id="5c4a1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="5c4a1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c4a1-133">Response</span></span>
<span data-ttu-id="5c4a1-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-134">The following is an example of the response.</span></span> <span data-ttu-id="5c4a1-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5c4a1-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c4a1-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
