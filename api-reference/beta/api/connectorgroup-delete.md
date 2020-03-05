---
title: Удаление Коннекторграуп
description: Удаление объекта Коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 960fe8a61dc00eaddcd6c96e255ea7cb7033434c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437485"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="f34f9-103">Удаление Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="f34f9-103">Delete connectorGroup</span></span>

<span data-ttu-id="f34f9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f34f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f34f9-105">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="f34f9-105">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="f34f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f34f9-106">Permissions</span></span>
<span data-ttu-id="f34f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f34f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f34f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f34f9-109">Permission type</span></span>      | <span data-ttu-id="f34f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f34f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f34f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f34f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f34f9-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f34f9-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f34f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f34f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f34f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f34f9-114">Not supported.</span></span>    |
|<span data-ttu-id="f34f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f34f9-115">Application</span></span> | <span data-ttu-id="f34f9-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f34f9-116">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f34f9-117">**Примечание:** У группы соединителей не должно быть связанных соединителей.</span><span class="sxs-lookup"><span data-stu-id="f34f9-117">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="f34f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f34f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f34f9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f34f9-119">Request headers</span></span>
| <span data-ttu-id="f34f9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f34f9-120">Name</span></span>       | <span data-ttu-id="f34f9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f34f9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f34f9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f34f9-122">Authorization</span></span>  | <span data-ttu-id="f34f9-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="f34f9-123">Bearer.</span></span> <span data-ttu-id="f34f9-124">Обязательна</span><span class="sxs-lookup"><span data-stu-id="f34f9-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f34f9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f34f9-125">Request body</span></span>
<span data-ttu-id="f34f9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f34f9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f34f9-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f34f9-127">Response</span></span>

<span data-ttu-id="f34f9-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f34f9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f34f9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f34f9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f34f9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f34f9-131">Request</span></span>
<span data-ttu-id="f34f9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f34f9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="f34f9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f34f9-133">Response</span></span>
<span data-ttu-id="f34f9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f34f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
