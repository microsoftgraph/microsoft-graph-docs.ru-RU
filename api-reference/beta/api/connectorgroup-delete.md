---
title: Удаление Коннекторграуп
description: Удаление объекта Коннекторграуп.
localization_priority: Normal
ms.openlocfilehash: 34bf5dd919ddea37f429e61fc9b01c1ee4c2d68c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327704"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="98af5-103">Удаление Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="98af5-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98af5-104">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="98af5-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="98af5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98af5-105">Permissions</span></span>
<span data-ttu-id="98af5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="98af5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98af5-108">Permission type</span></span>      | <span data-ttu-id="98af5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98af5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98af5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98af5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98af5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="98af5-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="98af5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98af5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98af5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98af5-113">Not supported.</span></span>    |
|<span data-ttu-id="98af5-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="98af5-114">Application</span></span> | <span data-ttu-id="98af5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98af5-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="98af5-116">**Примечание:** У группы соединителей не должно быть связанных соединителей.</span><span class="sxs-lookup"><span data-stu-id="98af5-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="98af5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98af5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="98af5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98af5-118">Request headers</span></span>
| <span data-ttu-id="98af5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="98af5-119">Name</span></span>       | <span data-ttu-id="98af5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="98af5-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="98af5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="98af5-121">Authorization</span></span>  | <span data-ttu-id="98af5-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="98af5-122">Bearer.</span></span> <span data-ttu-id="98af5-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="98af5-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="98af5-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98af5-124">Request body</span></span>
<span data-ttu-id="98af5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98af5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98af5-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="98af5-126">Response</span></span>

<span data-ttu-id="98af5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="98af5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98af5-129">Пример</span><span class="sxs-lookup"><span data-stu-id="98af5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98af5-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="98af5-130">Request</span></span>
<span data-ttu-id="98af5-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98af5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="98af5-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="98af5-132">Response</span></span>
<span data-ttu-id="98af5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98af5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
