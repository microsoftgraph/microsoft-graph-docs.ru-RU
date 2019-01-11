---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
localization_priority: Normal
ms.openlocfilehash: fbba85c9bb1807955670d19398e2175c3805f64f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851709"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="44c20-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="44c20-102">Enumerate lists in a site</span></span>

> <span data-ttu-id="44c20-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44c20-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44c20-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c20-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44c20-105">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="44c20-105">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="44c20-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44c20-108">Permissions</span></span>

<span data-ttu-id="44c20-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44c20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44c20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44c20-111">Permission type</span></span>      | <span data-ttu-id="44c20-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44c20-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44c20-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44c20-113">Delegated (work or school account)</span></span> | <span data-ttu-id="44c20-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44c20-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="44c20-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44c20-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c20-116">Not supported.</span></span>    |
|<span data-ttu-id="44c20-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44c20-117">Application</span></span> | <span data-ttu-id="44c20-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44c20-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44c20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44c20-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="44c20-120">Пример</span><span class="sxs-lookup"><span data-stu-id="44c20-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="44c20-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="44c20-121">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="44c20-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="44c20-122">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="44c20-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="44c20-123">Remarks</span></span>

<span data-ttu-id="44c20-124">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="44c20-124">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="44c20-125">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="44c20-125">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
