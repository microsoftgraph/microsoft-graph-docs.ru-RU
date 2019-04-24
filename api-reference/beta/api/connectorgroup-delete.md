---
title: Удаление Коннекторграуп
description: Удаление объекта Коннекторграуп.
localization_priority: Normal
ms.openlocfilehash: a0fd138281b8337df49388f4a10dc34cc02da18d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455914"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="9e9d4-103">Удаление Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="9e9d4-103">Delete connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e9d4-104">Удаление объекта Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-104">Delete a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="9e9d4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9d4-105">Permissions</span></span>
<span data-ttu-id="9e9d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e9d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e9d4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e9d4-108">Permission type</span></span>      | <span data-ttu-id="9e9d4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e9d4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e9d4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e9d4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e9d4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e9d4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e9d4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e9d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e9d4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-113">Not supported.</span></span>    |
|<span data-ttu-id="9e9d4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e9d4-114">Application</span></span> | <span data-ttu-id="9e9d4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e9d4-115">Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="9e9d4-116">**Примечание:** У группы соединителей не должно быть связанных соединителей.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-116">**Note:** The connector group must not have any connectors associated with it.</span></span>

## <a name="http-request"></a><span data-ttu-id="9e9d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e9d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9e9d4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e9d4-118">Request headers</span></span>
| <span data-ttu-id="9e9d4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9e9d4-119">Name</span></span>       | <span data-ttu-id="9e9d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9e9d4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e9d4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e9d4-121">Authorization</span></span>  | <span data-ttu-id="9e9d4-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-122">Bearer.</span></span> <span data-ttu-id="9e9d4-123">Обязательно</span><span class="sxs-lookup"><span data-stu-id="9e9d4-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e9d4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e9d4-124">Request body</span></span>
<span data-ttu-id="9e9d4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e9d4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9d4-126">Response</span></span>

<span data-ttu-id="9e9d4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e9d4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9e9d4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e9d4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e9d4-130">Request</span></span>
<span data-ttu-id="9e9d4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="9e9d4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e9d4-132">Response</span></span>
<span data-ttu-id="9e9d4-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e9d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
