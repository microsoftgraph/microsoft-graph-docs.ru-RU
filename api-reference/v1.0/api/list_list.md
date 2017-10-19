---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "Создание списка списков SharePoint на сайте"
ms.openlocfilehash: 4be4c4aefc29cdcd684bc11ad086b5c0572dbe2b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="55dfc-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="55dfc-102">Enumerate lists in a site</span></span>

<span data-ttu-id="55dfc-103">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="55dfc-103">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="55dfc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55dfc-106">Permissions</span></span>

<span data-ttu-id="55dfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55dfc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55dfc-109">Permission type</span></span>      | <span data-ttu-id="55dfc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55dfc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55dfc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55dfc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55dfc-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55dfc-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="55dfc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55dfc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55dfc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55dfc-114">Not supported.</span></span>    |
|<span data-ttu-id="55dfc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55dfc-115">Application</span></span> | <span data-ttu-id="55dfc-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55dfc-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55dfc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55dfc-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="55dfc-118">Пример</span><span class="sxs-lookup"><span data-stu-id="55dfc-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="55dfc-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="55dfc-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="55dfc-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="55dfc-120">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
